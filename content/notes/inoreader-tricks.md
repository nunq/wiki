# inoreader tricks

inoreader is my rss/feed/content reader of choice because it's literally the best. period.

## content views
* IMO column view is the most effective (but it took me some time to realize that)
* i group the items by feed, which i'd recommend if you have a lot of sources

## keep a log of your star history
* right-click read later section, choose get rss feed
* add that rss feed to inoreader and add a rule that auto reads that feed

## filter a feed
* use the filter feature, not rules. from my experience filters are processed before rules

## word filter a folder
* use a new article in folder rule

## global account word filter
* use a new article in account rule

## twitter timeline
* you can subscribe to your twitter timeline by adding https://twitter.com/home (you have to add your twt acc in the settings)

## keyboad shortcuts
* enable them in `settings > other > power user settings`

### examples
* `h` show help
* `g-a` goto all articles
* `g-d` goto dashboard
* `g-f` goto starred articles
* `v` open article in new tab (foreground)
* `b` open in bg
* `shift-1` show only unread articles
* `shift-2` show all articles
* `shift-a` mark all as read
* `r` refresh
* `f` star article
* `j`/`k` move one article down/up

## custom css
can be added in `settings > other > power user settings`. here's mine:
```css
/* hide prev/next article/refresh buttons in top bar (right) */
#sb_rp_prev_article, #sb_rp_next_article, #sb_rp_refresh {
  display: none;
}
/* hide ugly eye button in sidebar */ 
#subscription_options_peek_wrapper {
  display: none;
}
```

## etc
* duplicate filters for news or technology folders are great because news publications often publish the same things and hackernews and lobsters content has overlap too
* for newsletters: either built-in feature or https://kill-the-newsletter.com
