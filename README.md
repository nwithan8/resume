# Nate Harris' Resume

---

## Resume

### [PDF Version](https://github.com/nwithan8/resume/blob/master/resume.pdf)

## CV

### [Digital Version](https://registry.jsonresume.org/nwithan8?theme=kendall)

### [PDF Version](https://github.com/nwithan8/resume/blob/master/cv.pdf)

---

## How it works

This CV is stored as JSON following the [JSON Resume schema](https://raw.githubusercontent.com/jsonresume/resume-schema/v1.0.0/schema.json). When changes are committed, GitHub Actions copies the JSON file to a [Gist](https://gist.github.com/nwithan8/65f296251b18fca7f443268578a8529f), which is then picked up by the [JSON Resume Registry](https://jsonresume.org/getting-started/).

The multi-page "cv.pdf" file is then [auto-generated](#saving-pdf) using the `resume-cli` tool and copied to the repository.

The single page "resume.pdf" file is manually written.

#### Saving PDF

There are two CLI tools, `resume-cli` via NPM and `resumed` via GitHub, neither of which work great, especially with PDF conversion.

To save the resume as a PDF, first download a theme that will produce a thin rendered page (I recommend the [BufferBloat](https://www.npmjs.com/package/jsonresume-theme-bufferbloat) theme). Install the `resume-cli` tool via NPM, and run `resume --theme bufferbloat serve` to run a local webserver. Navigate to `localhost:4000` and print the page to "Save as PDF".
