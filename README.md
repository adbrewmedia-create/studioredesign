# Studio redesign prototype

One static page (index.html), no build step. All data is sample data held in the
browser; a refresh resets it. Decks, videos and sites have their own links (#deck-1, #deck-1-edit, #video-1, #site-11).

Deploy as its own Vercel project so it does not touch the live Studio app:

    cd studio-redesign
    npx vercel@latest deploy --prod

The first run asks you to log in and to name the project (e.g. studio-redesign).
vercel.json marks the site noindex so search engines leave it alone.
