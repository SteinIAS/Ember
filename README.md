![Ember](https://s4.postimg.org/ec3ncyzb1/Ember-_Template.jpg)

# Ember
A best practise email template to be used as a starter kit for new emails.

## Best Practice Techniques
**Don't** use `<br />` tags for spacing, create single cell rows with a `<td></td>` inside instead so you can control the spacing through border, padding-top or bottom etc. Also this allows individual paragraphs to be styled differently (eg: center align, bigger fonts etc) by non-devs

```html
<tr>
	<td align="left" valign="top" style="padding-top: 10px; padding-bottom: 10px;">Example Text 1</td>
</tr>
<tr>
	<td align="left" valign="top" style="padding-top: 10px; padding-bottom: 10px;">Example Text 2</td>
</tr>
```
---

Always add a `valign` attrbute on all `<td>` tags, for best practice and consistency.

---

When we want two elements next to each other on desktop but want them to stack on mobile, we use `<th></th>` tags instead of `<td></td>` to work acorss all devices, this is to fix the latest IOS versions.

```html
<tr>
	<th align="left" valign="top" style="width: 300px; padding-bottom: 10px; padding-top: 10px; vertical-align: top; font-weight: normal;" class="fullWidth align-center"></th>
	<th align="right" valign="top" style="width: 300px; padding-bottom: 10px; padding-top: 10px; vertical-align: top; font-weight: normal;" class="fullWidth align-center"></th>
</tr>
```

---

Don't forget to change the `<title></title>` tags value on each email to fit the campaign/client intended instead of leaving it to the default **Ember Template**

---

All `<img>` tags must look like the below example, missing these attributes out can cause issues across clients. i.e. Styling, alt tags etc.

```html
<img src="http://placehold.it/200x200" width="100" height="100" alt="placeholder" style="border: none; outline: none;" />
```

Images are always 2x there size also, so if you have an image that is both 200px width and height. You would set the width and height to be `width="100" height="100"` so that it's retina friendly/mobile proof.

---

When using anchor links across your email, you need to include the styling as shown below so that it doesn't display unusual borders or outlines across some clients.

```html
<a href="http://www.google.co.uk" style="outline: none; border: none; text-decoration: none; color: #000000;" target="_blank">Google</a>
```

### HAPPY CODING!

