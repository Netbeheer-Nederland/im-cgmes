# CGMES Profiles

## Re-generating Documentation
1. Have a virtual environment active which has `linkml`, `mkdocs`, `mkdocs-material` and `pyyaml` installed
2. Change working directory to `./documentation`
3. Clear the `_docs` directory of all `.md` files, **but keep the `assets` subdirectory**:
```shell
$ rm _docs/*.md
```
4. Generate the static Markdown files:
```shell
$ gen-doc -d _docs/ --diagram-type uml_class_diagram --template-directory _templates/ --use-slot-uris /path/to/your_schema.yaml
```
5. Generate the static HTML website:
```shell
$ mkdocs build
```
6. Delete slot and type pages, since these cause problems and don't provide us anything meaningful for the CGMES profiles. To do this, first change the working directory to `_docs` and then run:
```shell
$ grep '^# Slot: ' -e '^# Type: ' *.md -l | xargs rm
```
7. CIM primitive types are standard classes for which pages are created also, but since we map these types onto LinkML primitive types, we can remove these pages also. Most were overwritten by LinkML native types, but you need to delete `DateTime.md` and `MonthDay.md` manually.
8. The index page has some references to LinkML and CIM primitive data types that we need to remove manually. Running `mkdocs build` again tells you what the dead references are (LinkML types). The others are `DateTime` and `MonthDay` from CIM. Remove these entries from the classes table in `_docs/index.md` and build again.
