#ByJC-CV

Here is my CV in JSON Format build with the [JSON Resume](https://jsonresume.org)
you can find a demo [here](http://registry.jsonresume.org/ByJC)

# resume-cli


This is the command line tool for [JSON Resume](https://jsonresume.org/), the open source initiative to create a JSON-based standard for resumes.

[Read more...](https://jsonresume.org/schema/)

# Getting Started

```
npm install -g resume-cli
```

# Usage

```
resume --help
```

For a complete list of options and commands.

```
resume init
```

Creates a new resume.json file in your current working directory.   

Complete the resume.json with your text editor, following the schema available at:  
http://jsonresume.org/

```
resume test
```

Runs your resume.json through our schema tests to ensure it complies with the standard and tries to identify where any errors may be occurring.

```
resume export [fileName]
```

Exports your resume locally in a stylized html, markdown, or pdf format.

Use the `--format` flag to specify file type. Example: `--format pdf`

Use the `--theme <name>` flag to specify theme. Example: `--theme flat`  
_A list of available themes can be found here: http://jsonresume.org/themes/_

```
resume register
```

_Registration is optional._

To publish your resume to your account with a custom domain extension at http://registry.jsonresume.org/, you will first need to acquire login credentials. 

```
resume publish
```

This command will guide you through the publish process.
Consider using the theme flag to style your resume (Default: `flat`).

Example: `resume publish --theme flat`

```
resume serve
```

Starts a web server that serves your local resume.json.  
Options: `--port <port>`, `--theme <name>`

If no theme is specified, it will try to locate a local `index.js` and call the `render()` function. This is useful when developing themes.

## License

Available under [the MIT license](http://mths.be/mit).