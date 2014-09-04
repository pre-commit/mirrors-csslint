csslint mirror
================

Mirror of csslint package for pre-commit.

For pre-commit: see https://github.com/pre-commit/pre-commit

For jshint: see https://github.com/CSSLint/csslint


### Using csslint with pre-commit

Add this to your `.pre-commit-config.yaml`:

    -   repo: git://github.com/pre-commit/mirrors-csslint
        sha: ''  # Use the sha you want to point at
        hooks:
        -   id: csslint

Note that csslint does not exit with a non-zero return code
unless the issue is an error. A lot of common mistakes are
considered warnings. We suggest you add a .csslintrc file
to your project. See https://github.com/CSSLint/csslint/wiki/Command-line-interface#configuration-files
