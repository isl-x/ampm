# ampmdc.co

## Installation

    $ bundle install

    $ npm install

## Local Development

Build Jekyll into `_site`:

    $ grunt build

Build Jekyll and run [htmlproofer](https://github.com/gjtorikian/html-proofer)
on `_site`:

    $ grunt test

Serve `_site` at <http://localhost:8000>, livereload expanded sass changes,
rebuild Jekyll as needed:

    $ grunt serve

Parse `_sass`, `css`, and `js` for [Modernizr](http://modernizr.com/)
references and build to `js/lib/modernizr.min.js`:

    $ grunt modernizr

## Deployment

    $ git push origin gh-pages

## Email

1. Images for the emails are stored in the `img/email` folder. The email templates
reference the URL of those images.
1. Templates for the emails are in the `html-email` orphan branch of this
   project.
1. We aren't using the email builder yet, but the structure is there to do so.
1. For now, just log into [Litmus](https://litmus.com) with the antimatter
   creds and edit the template that is already there.
1. Once everything is tested, download the packaged assets from Litmus.
1. The zip file can be uploaded directly to [MailChimp](http://mailchimp.com/)
   (creds are specific to the AMPM project. Not the regular dev creds.)
1. The html file itself is currently just backed up to github. Location is
   `/dist/` folder in the `html-email` branch.
