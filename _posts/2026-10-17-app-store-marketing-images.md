---
layout: post
title: Designing assets for Apple's new App Store display options
lang: en
image: /images/appstore-connect-hero-preview.jpg
---

With the release of iOS 27, App Store Connect introduced **new options for displaying custom assets** at the top of your app's App Store page, and in place of the first three screenshots in the search results page.

I think this is an underrated opportunity to stand out right now, since not many apps appear to use these new options.

I have created and uploaded custom assets for [my read-later app Flyleaf](/) and I want to talk about what I've learned, and what works well and what doesn't in my opinion.

First of all, you need to upload any assets you want to use in App Store Connect, in the new "Content library" section. This is all fairly self-explanatory, but I have some tips:

- The upload will fail with a nondescript error message if the **dimensions of your file** are not *exactly* as required. The safest way I found to get this right is to download one of the templates from [developer.apple.com/app-store/asset-best-practices/](https://developer.apple.com/app-store/asset-best-practices/) and use them as a basis
- The templates also include a **"safe area" layer**. It's not obvious, but this is only the smallest part of the image that is *guaranteed* to be displayed. But it's *way* tighter than the area that will typically be visible to users, even on small devices.[^1]
- On the other hand, pay attention to the composition of your asset, because the App Store will not just display the largest possible portion of your asset – it will always be somewhat zoomed in.
- The best way to experiment with how the different devices will frame your asset is to try it out in the **preview provided by App Store Connect**. The preview matches the final result visitors will see pretty well, in my experience.
- Annoyingly, any asset you want to preview first has to be uploaded *and reviewed* by App Review. This can take several hours, but at least you can send in assets for review without updating your app. Anyway, I would prepare several asset variants upfront. That way, if one doesn't look right in the previews, you already have alternatives ready.

![Screenshot of the new App Store Connect preview for marketing assets](/images/appstore-connect-hero-preview.jpg)

[^1]: I think it's only when you pull down as far as possible on a product page that the image gets zoomed in to the dimensions of the safe area.

Let's talk about the actual content of the assets. I think you should use different kinds of artwork for the search results and the product page

### Custom assets for search results

In search results, the custom asset replaces the row of screenshots that would have been displayed previously. This is a great opportunity to craft an asset that shows off your app in its best light. You should probably include at least one screenshot in the asset, because otherwise users will not see what your app looks like until they tap your listing.

On the other hand, you probably should not include your apps name or icon in the asset, because they're already displayed right above it. If you had text in your hero screenshots, you could include it here, as well.

Here is what I went with for Flyleaf:

![](/images/Flyleaf_AppStoreHero_4-screenshot.jpg)

And, to get a feel for how the image is cropped, here is the source image:

![](/images/Flyleaf_AppStoreHero_4.jpg)

### Custom assets for the product page

The product page is a slightly different matter. This one is less about showcasing your app and more about conveying the "vibe" or theme of your app.

You probably don't want your hero asset to distract too much from the actual content of your product page. Also, because the product page has its own screenshots, there is not much point in including a device or screenshots in the product page header asset.

This is the image I went with for Flyleaf:

![](/images/Flyleaf_AppStoreHero_4-nodevice-screenshot.jpg)

One thing to watch out for: The top of the asset behind the iPhone notch will annoyingly be blurred *and mirrored* instead of just using the image data that's clearly already there. So don't put anything too distracting at the top of your asset, I guess.

Again, here is the source image:

![](/images/Flyleaf_AppStoreHero_4-nodevice.jpg)

Another very tasteful example is this one for [Pockity by Nikhil Nigade](https://social.dezinezync.com/@nikhil/117454481514432891):

<div style="margin: 1rem auto; max-width: 500px;">
<blockquote class="mastodon-embed" data-embed-url="https://social.dezinezync.com/@nikhil/117454481514432891/embed" style="background: #FCF8FF; border-radius: 8px; border: 1px solid #C9C4DA; margin: 0; max-width: 540px; min-width: 270px; overflow: hidden; padding: 0;"> <a href="https://social.dezinezync.com/@nikhil/117454481514432891" target="_blank" style="align-items: center; color: #1C1A25; display: flex; flex-direction: column; font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Oxygen, Ubuntu, Cantarell, 'Fira Sans', 'Droid Sans', 'Helvetica Neue', Roboto, sans-serif; font-size: 14px; justify-content: center; letter-spacing: 0.25px; line-height: 20px; padding: 24px; text-decoration: none;"> <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="32" height="32" viewBox="0 0 79 75"><path d="M63 45.3v-20c0-4.1-1-7.3-3.2-9.7-2.1-2.4-5-3.7-8.5-3.7-4.1 0-7.2 1.6-9.3 4.7l-2 3.3-2-3.3c-2-3.1-5.1-4.7-9.2-4.7-3.5 0-6.4 1.3-8.6 3.7-2.1 2.4-3.1 5.6-3.1 9.7v20h8V25.9c0-4.1 1.7-6.2 5.2-6.2 3.8 0 5.8 2.5 5.8 7.4V37.7H44V27.1c0-4.9 1.9-7.4 5.8-7.4 3.5 0 5.2 2.1 5.2 6.2V45.3h8ZM74.7 16.6c.6 6 .1 15.7.1 17.3 0 .5-.1 4.8-.1 5.3-.7 11.5-8 16-15.6 17.5-.1 0-.2 0-.3 0-4.9 1-10 1.2-14.9 1.4-1.2 0-2.4 0-3.6 0-4.8 0-9.7-.6-14.4-1.7-.1 0-.1 0-.1 0s-.1 0-.1 0 0 .1 0 .1 0 0 0 0c.1 1.6.4 3.1 1 4.5.6 1.7 2.9 5.7 11.4 5.7 5 0 9.9-.6 14.8-1.7 0 0 0 0 0 0 .1 0 .1 0 .1 0 0 .1 0 .1 0 .1.1 0 .1 0 .1.1v5.6s0 .1-.1.1c0 0 0 0 0 .1-1.6 1.1-3.7 1.7-5.6 2.3-.8.3-1.6.5-2.4.7-7.5 1.7-15.4 1.3-22.7-1.2-6.8-2.4-13.8-8.2-15.5-15.2-.9-3.8-1.6-7.6-1.9-11.5-.6-5.8-.6-11.7-.8-17.5C3.9 24.5 4 20 4.9 16 6.7 7.9 14.1 2.2 22.3 1c1.4-.2 4.1-1 16.5-1h.1C51.4 0 56.7.8 58.1 1c8.4 1.2 15.5 7.5 16.6 15.6Z" fill="currentColor"/></svg> <div style="color: #787588; margin-top: 16px;">Post by @nikhil@social.dezinezync.com</div> <div style="font-weight: 500;">View on Mastodon</div> </a> </blockquote> <script data-allowed-prefixes="https://social.dezinezync.com/" async src="https://social.dezinezync.com/embed.js"></script>
</div>

----

You can see these assets in action on [Flyleaf's App Store page](). Give the app a try if you haven't already!

{% include flyleaf-download.html %}