# GroupDocs.Annotation Landing Pages

This repository contains the files used to generate GroupDocs.Annotation landing pages e.g. <https://products.groupdocs.com/annotation/net/add/docx/>

## Prerequisites

* Install Hugo and related tools

    `npm install -g hugo-extended postcss postcss-cli autoprefixer`

* Clone `common` submodule that contains theme for the landing pages

    `git submodule update --recursive --init`

## Running

* Copy files from `.\english` folder to `common\content\english`

* Navigate in `common` folder

* Execute `hugo server` or `hugo server -b products.groupdocs.com` to build pages and start Hugo server

## Publishing

Commit your changes or create pull request into `master` branch and GitHub actions will do the rest.
