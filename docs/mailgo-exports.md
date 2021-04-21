---
id: mailgo-exports
title: Mailgo export(s)
sidebar_label: Library export(s)
---

Here the functions exported by the library `mailgo`

```js
export {
  getMailgoTypeByElement,
  mailgoClickListener,
  mailgoCheckRender, // DEPRECATED, is now mailgoClickListener
  mailgoPreRender,
  mailgoDirectRender,
  mailgoRender,
  mailgoValidateEmail,
  mailgo,
  start, // same as mailgo
};

export default mailgo;
```

## Definitions

### getMailgoTypeByElement

```ts
export function getMailgoTypeByElement(
  element: HTMLElement
): MailgoModalType | null;
```

// TODO: more documentation here will arrive soon!

### mailgoClickListener (or DEPRECATED mailgoCheckRender)

```ts
export function mailgoClickListener(event: Event): boolean;
```

// TODO: more documentation here will arrive soon!

### mailgoPreRender

```ts
export function mailgoPreRender(
  type: string,
  mailgoElementOrUrl: HTMLLinkElement | string
): boolean;
```

// TODO: more documentation here will arrive soon!

### mailgoDirectRender

```ts
export function mailgoDirectRender(directUrl: string): boolean;
```

// TODO: more documentation here will arrive soon!

### mailgoRender

```ts
export function mailgoRender(type: string): boolean;
```

// TODO: more documentation here will arrive soon!

### mailgoValidateEmail

```ts
export function mailgoValidateEmail(email: string): boolean;
```

Validates an email address through the same validation function (i.e. same `RegExp`) used internally by mailgo.

It could be useful to call this function if, for example, you want to notify the user of an invalid To: address before calling the `mailgoDirectRender` function. In this way the validation of the email address can be performed in the same way as mailgo does.

### mailgo

```ts
export default function mailgo(mailgoConfig?: MailgoConfig): boolean;
```

// TODO: more documentation here will arrive soon!
