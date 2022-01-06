PATH := ./scripts/bin:$(PATH)
export APP_SCRIPTS := scripts
export APP_ARGS := -e -s --headless
export APP_HOME := ./scripts


# NOTE: notation
targets : prerequisites
    recipe
    ...

targets : prerequisites ; recipe
    recipe
    ...

# Variable assignment
# -------------------
# variables defined with `=` are *recursively expanded variables*
# variables defined with `:=` or `::=` are *simply expanded variables*; they contain variable *references* that will be
#       expanded before the definition is made.
# FOO ?= bar    set variable *only if* variable FOO is not already set.
# Shell assignment:
#       FOO != <output of shell command>


install:
    pip install --upgrade app-name  # TODO: set `app-name`

test:
    pytest3 -vv     

pdf:
    asciidoctor-pdf ./docs/_static/main.adoc

python-app:
    git clone https://github.com/reecechimento/app-name app-name  # TODO: set `app-name`

.PHONY: install test pdf
# NOTE: common PHONY ``make`` targets: all, install, clean, distclean, TAGS, info, check
