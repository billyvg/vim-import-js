# Vim support

ImportJS is meant to be used as a Pathogen plugin. Just `git clone` this repo
into the `bundles` folder and you are good to go!

## Dependencies

You need to have the import-js npm package installed to use this plugin.

```sh
npm install -g import-js
```

## Speeding it up with Watchman

If you want an extra performance boost, you can [install
Watchman](https://facebook.github.io/watchman/docs/install.html). See the
[ImportJS
README](https://github.com/Galooshi/import-js#speeding-it-up)
for more information.

## Default mappings

By default, ImportJS attempts to set up the following mappings:

Mapping     | Command               | Description
------------|-----------------------|---------------------------------------------------------------------
`<Leader>j` | `:ImportJSWord`       | Import the module for the variable under the cursor.
`<Leader>i` | `:ImportJSFix`        | Import any missing modules and remove any modules that are not used.
`<Leader>g` | `:ImportJSGoto`       | Go to the module of the variable under the cursor.

## Troubleshooting

If you run into issues when using the plugin, adding some logging can help.
After starting up vim, and before you've imported anything, run this command:

```
:call ch_logfile('channel_log.txt', 'w')
```

After this, you will get useful information in `channel_log.txt`.
