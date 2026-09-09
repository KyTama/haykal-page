# Static deployment boundary

For a portable single-file site, publish the reviewed HTML unchanged as `index.html` and keep deployment configuration beside it. GitHub Pages can serve the document directly without a build step, which avoids introducing a second asset pipeline or changing embedded identity assets.

Keep the source design file outside the deployment copy. Verify byte equality immediately after copying, then verify the deployed response separately because source integrity and hosting configuration are different failure surfaces.
