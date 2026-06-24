<h2>Skin breakdown</h2>

**Layout & Background**
- `html`, `body`, `body::before`, `body::after` — sets up the full-page background image and makes everything else sit on top of it transparently

**Header**
- `#header` — the top bar layout (flexbox, spacing)
- `#header h1.heading` — replaces the AO3 logo with your custom image
- `#header ul.primary` — the main nav links (Browse, People, etc.)
- `#header .search` — the search bar in the header
- `#greeting` — the user menu area (your username, inbox, logout icons)

**Footer**
- `#footer` — the bottom bar styling

**Dashboard (sidebar)**
- `#dashboard` — the left sidebar navigation on your profile/works pages
- `#dashboard .current` — the currently active sidebar link

**Work blurbs (listing cards)**
- `ol.index:not(.listbox) > li.blurb` — the bordered cards on browse/search pages
- `li.work.blurb`, `li.series.blurb`, `li.bookmark.blurb` — individual work/series/bookmark cards
- `.listbox li.blurb` — blurbs inside listboxes (simpler style)

**Tags**
- `a.tag` — general tag pill styling
- `.warnings .tag` — archive warning tags (green)
- `.relationships .tag` — relationship tags (light green)
- `.characters .tag` — character tags (pale green)
- `.freeforms .tag` — additional tags (lightest green)
- `dd.rating a.tag`, `dd.category a.tag` — rating and category tags (warm beige tones)
- `ul.tags li.warnings:first-child:before` etc. — the ☘️/🍀 label prefixes before each tag group

**Required tags icons (the little symbol badges)**
- `.blurb ul.required-tags li .rating` etc. — the small G/T/M/E rating and ⚣/⚢ category badges
- `.rating-general-audience`, `.rating-mature` etc. — color coding for each rating/category

**Stats icons**
- `dl.stats dd::before` — the little icon shown before each stat (words, kudos, hits, etc.)
- Each `dl.stats dd:nth-of-type` or named class like `.kudos`, `.hits` — maps a specific Tumblr-hosted icon image to each stat type

**Work skin (the reading page)**
- `#workskin` — the bordered frame around fic content
- `#workskin > .userstuff` — the actual fic text area
- `#workskin h2.title`, `h3.byline` — title and author line centering
- `.userstuff hr::before` — replaces `<hr>` dividers with your `ʚ🍏✧🍏ɞ` string

**Comments**
- `li.comment` — the comment card box
- `.comment div.icon` — the avatar box in a comment
- `.comment .userstuff` — the text body of a comment
- `.thread .even` — nested/reply comment shading
- `.replied`, `span.unread` — replied/unread badges

**Kudos section**
- `p.kudos` — the kudos list box with the decorative background image
- `#kudos_message.notice::before` — replaces the "kudos left!" confirmation with your custom magic message
- `#kudos_message.kudos_error::before` — replaces the "already left kudos" error with your custom spell message

**Subscriptions**
- `dl.subscription.index.group` — the subscriptions list on your My Subscriptions page

**Bookmarks**
- `li.bookmark.blurb` — bookmark cards
- `.bookmark .user` — the user info section inside a bookmark
- `.bookmark .status span` — the bookmark status icons (public/private/rec)

**Collections**
- `ol.collection.index li.collection.blurb.group` — collection cards
- `li.mystery.blurb.group` — anonymous/mystery collection entries

**Pagination**
- `.pagination .current` — the current page number button
- `.pagination li a` — other page number buttons

**Forms & filters**
- `form.filters fieldset` — the filter sidebar on browse pages
- `input`, `textarea`, `select` — all form fields
- `input[type="checkbox"]`, `input[type=radio]` — custom checkbox/radio styling
- `.filters .indicator` — the custom checkbox indicators in filters

**Notifications/alerts**
- `.notice`, `.error`, `.alert.flash` — general notice/error boxes
- `.reading h4.viewed` — the "last visited" marker on works in your history

**Profile/user pages**
- `.bio.module` — your profile bio box
- `#main.users-edit` etc. — settings/edit pages
- `dl.meta` — metadata display lists

**Stat chart (statistics modal)**
- `#stat_chart` — the bar chart on your statistics page
- `.statistics.modal` — the stats popup modal

**Miscellaneous**
- `.pagination` — page navigation
- `.actions a`, `button`, `input[type="submit"]` — all buttons sitewide
- `span.question` — the little `?` help tooltip bubbles
- `p.kudos a[href="/users/airively"]` — bolds your own username in kudos lists

**Text selection color**
::selection {
  background: #aac8a9 !important;
  color: #57310D !important;
}

::-moz-selection {
  background: #aac8a9 !important;
  color: #57310D !important;
}
