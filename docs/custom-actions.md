---
id: custom-actions
title: Mailgo custom actions
sidebar_label: Custom actions
---

From version `0.12.*` it is possible to pass a custom url to the mailgo element and have it rendered as a custom action in the modal.

To add a custom action, the `data-custom-action-text` and `data-custom-action-url` attributes need to be specified in the mailgo element, like this:

```html
<a href="mailto:info@mailgo.dev" data-custom-action-text="Open Docs" data-custom-action-url="https://mailgo.dev/docs/">info@mailgo.dev</a>
```

<a href="mailto:info@mailgo.dev" data-custom-action-text="Open Docs" data-custom-action-url="https://mailgo.dev/docs/">info@mailgo.dev</a>

With the example `mailto:` link above, when the mailgo modal opens it will also show an additional link whose text will be "Open Docs" and which, when clicked, will open a new browser tab with the url https://mailgo.dev/docs/.

In order for custom actions to work the `custom` action should be enabled in the mailgo config (by default it is enabled).

Custom actions will only work when mailgo is used with `mailto:` links. So it is not supported, at least for now, with `tel:` or `callto:` links and with `mailgoDirectRender`.
