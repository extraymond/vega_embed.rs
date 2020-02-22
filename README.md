# vega-embed-shim

This is a utility crate to let vega-embed-rs to call the vega-embed.js library to render it's spec.

The purpose of this crate:
1. Allow user to reuse their vega-lite chart generated from the vega-lite-3 crate,
2. Render the chart onto their rust/frontend using web_sys::Element as a target.

Prerequisite:
1. Make sure the required library for vega-embed is loaded in the header of your html file.
2. Make sure you have allocated enough stack memory so that the vega-lite-3 chart won't stuff your wasm memory pool.