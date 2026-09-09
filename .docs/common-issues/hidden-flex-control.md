# Hidden controls need an explicit author-level rule

An element with the HTML hidden attribute can still appear when an author stylesheet gives that same element a display value such as flex or grid. The result is worse than a visual mismatch when the exposed descendant remains focusable and editable.

For conditionally rendered controls, pair the hidden attribute with a component-level hidden selector and disable inactive form fields in state synchronization. Verify the accessibility tree in both directions of the toggle, not only the screenshot.
