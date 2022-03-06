# AServe-CLP v1.0
Patch that allows CLP Web Page templates to work with latest (2019) Portable AllegroServe (v1.2.60).

Currently being used in my production websites served from `:aserve` and using `:webactions`

## Usage

1. Place / copy the file `clpage-patch.lisp` directly into your project directory (or anywhere in your project path).
2. Edit your .asd to similar to the following:

```
(defsystem "project-name"
  :version "0.1.0"
  :author "First Surname"
  :license ""
  :depends-on ("aserve" "webactions")
  :components ((:file "clpage-patch")
  ...
```
3. Load your project and start using Webactions with CLP templates.
