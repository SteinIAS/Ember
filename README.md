# Ember
A best practise email template to be used as a starter kit for new emails.

## Best Practice Techniques
**Don't** use `<br />` tags for spacing, create single cell rows with a `<td></td>` inside instead so you can control the spacing through border, padding-top or bottom etc.

```html
<tr>
	<td align="left" valign="top" style="padding-top: 10px; padding-bottom: 10px;">Example Text</td>
</tr>
```
---

Always add a `valign` attrbute on all `<td>` tags, for best pratice and consistency.

---

When we want two elements next to each other to stack on mobile, we use `<th></th>` tags instead of `<td></td>` to work acorss all devices, this is to fix the latest IOS versions. 

```html
<tr>
	<th align="left" valign="top" style="width: 300px; padding-bottom: 10px; padding-top: 10px; vertical-align: top; font-weight: normal;" class="fullWidth align-center"></th>
	<th align="right" valign="top" style="width: 300px; padding-bottom: 10px; padding-top: 10px; vertical-align: top; font-weight: normal;" class="fullWidth align-center"></th>
</tr>
```

---

Don't forget to change the `<title></title>` attribute value on each email to fit the campaign/client intended instead of leaving it to the default **Ember Template**
