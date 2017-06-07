# Ember
A best practise email template to be used as a starter kit for new emails.

## Best Practice Techniques
**Don't** use `<br />` tags for spacing, create single cell rows with a td inside instead so you can control the spacing through border, padding-top or bottom etc.

```html
<tr>
	<td align="left" valign="top" style="padding-top: 10px; padding-bottom: 10px;">Example Text</td>
</tr>
```
======

> We want to add a `valign` attrbute on all `<td>` tags.
