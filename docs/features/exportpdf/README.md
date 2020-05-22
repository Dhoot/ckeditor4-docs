---
category: working-with-document
order: 25
url: features/exportpdf
menu-title: Export to PDF
meta-title-short: Export to PDF
---
<!--
Copyright (c) 2003-2020, CKSource - Frederico Knabben. All rights reserved.
For licensing, see LICENSE.md.
-->

# Exporting content to PDF

<info-box info="">
	This feature is provided through the [Export to PDF](https://ckeditor.com/cke4/addon/exportpdf) plugin that is not included in any official CKEditor 4 preset. You can {@link guide/dev/plugins/README add it to your custom build} with [online builder](https://ckeditor.com/cke4/builder) or download as a [npm package](https://www.npmjs.com/package/ckeditor4-plugin-exportpdf).
</info-box>

The [Export to PDF](https://ckeditor.com/cke4/addon/pastefromword) plugin allows you to export the content from editor to a PDF file.

{@img assets/img/exportpdf_01.png Export to PDF button.}

When enabled, it adds the **<img class="inline" src="%BASE_PATH%/assets/img/exportpdf-button.png" alt="Export to PDF toolbar button">Export to PDF** toolbar button. It sends data from editor to the endpoint maintained by [CKEditor Cloud Services](https://ckeditor.com/ckeditor-cloud-services/) and handles the response, saving it as a PDF file.

## Feature overview

Although CKEditor 4 is basically a web tool, sometimes you may want (or *need*) to use the content it generated somewhere else. While simple copy and paste may work in some cases, most probably it will not allow you to use some more advanced editor features like styled tables or lists. Thanks to the [Export to PDF](https://ckeditor.com/cke4/addon/pastefromword) plugin you can save the document you created to a downloadable file, preserving all the styles and structure in nearly 1:1 projection.

## Supported features

Plugin maintains all the formatting and content structure you create using the editor. See the tips for {@link features/exportpdf/README#optimal-projection obtaining the optimal projection} to learn how to configure the plugin to best suite your needs.

As for the compatibility, plugin works on all the browsers {@link guide/dev/browsers/README supported for CKEditor 4} except for Internet Explorer older than 11.

## A few "How to" guides

1.  Best projection (setting editor width - #14).
2.  Sync and async data processing (`pdfExport` event).
3.  Dynamic file naming (#13).
4.  Reference [endpoint docs](https://pdf-converter.cke-cs.com/docs).

## Export to PDF demo

See the {@linkexample exportpdf working "Export to PDF" sample} that showcases the export to PDF process.

## Related Features

Refer to the following resources for more information about working with document in CKEditor 4:

* {@link features/size/README Setting editor size} will allow you to obtain the closest to 1:1 projection.
* See the {@link guide/dev/acf/README content filtering} article to make editor work also with custom plugins.