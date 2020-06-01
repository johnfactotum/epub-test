# EPUB Test

An EPUB file to test various (mainly security) aspects of e-book readers.

## Usage

### Generating the EPUB file

```
cd epub-test
zip -rX ../epub-test.epub mimetype META-INF/ EPUB/
```

### Testing e-book readers with the EPUB file

EPUB files can contain JavaScript and other potentially dangerous contents. While many of these are allowed by the EPUB spec, they can cause serious security issues if not properly handled.

Currently this file does not do anything fancy. It contains simple things like:

- Links, forms, images, iframes, and CSS connecting to external resources
- Connecting to local files and external resources with JavaScript
