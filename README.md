# webseer

## Google Autocomple API exploration

### 1) Autocomplete result with HTML tag

#### Request URL：
  `GET` https://www.google.com/complete/search?q=`search-term`&cp=9&client=psy-ab&xssi=t&gs_ri=gws-wiz&hl=en&authuser=0&psi=CJ_gW_DkGfKJggfMyLqwDA.1541447435311&ei=CJ_gW_DkGfKJggfMyLqwDA&gs_mss=xwfe

#### Headers:
  None

#### Sample Response with `search-term==t`:
```
)]}'
[[["t\u003cb\u003earget\u003c\/b\u003e",0,[131]],["t\u003cb\u003eranslate\u003c\/b\u003e",0,[131]],["t\u003cb\u003ehe grinch\u003c\/b\u003e",0,[131]],["t\u003cb\u003erump\u003c\/b\u003e",0,[131]],["t\u003cb\u003ewitter\u003c\/b\u003e",0,[131]],["t\u003cb\u003eractor supply\u003c\/b\u003e",0,[131]],["t\u003cb\u003eicketmaster\u003c\/b\u003e",0,[131]],["t\u003cb\u003ehesaurus\u003c\/b\u003e",0],["t\u003cb\u003eutuapp\u003c\/b\u003e",0,[131]],["t\u003cb\u003ewitch\u003c\/b\u003e",0,[131]]],{"i":"xwfe","q":"1qr_JWuOmlR8R_DwfH7mXil7Mjs"}]
```
response are Unicode-encoded json list (with problaby prepended 4 char):
```json
[
	[
		[
			"t<b>arget</b>",
			0, [131]
		],
		[
			"t<b>ranslate</b>",
			0, [131]
		],
		[
			"t<b>he grinch</b>",
			0, [131]
		],
		[
			"t<b>rump</b>",
			0, [131]
		],
		[
			"t<b>witter</b>",
			0, [131]
		],
		[
			"t<b>ractor supply</b>",
			0, [131]
		],
		[
			"t<b>icketmaster</b>",
			0, [131]
		],
		[
			"t<b>hesaurus</b>",
			0
		],
		[
			"t<b>utuapp</b>",
			0, [131]
		],
		[
			"t<b>witch</b>",
			0, [131]
		],
	{
		"i": "xwfe",
		"q": "1qr_JWuOmlR8R_DwfH7mXil7Mjs"
	}
]
```
