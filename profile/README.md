## Hi there 👋

If you've been invited to this organization, it's probably because you signed up for my [mailing list on jacobparis.com](https://www.jacobparis.com). Welcome! You're an insider now!

> If you signed up and have not gotten an invite, it's very possible I just haven't gotten around to sending them yet. It's still a manual process. Either way – reply to any of my emails and I'll get you sorted. If you've subscribed with a different email than your GitHub, we can sort that out via email as well.

I made this org as a way to share the source of all the example projects I've built for each of my articles and tutorials.

Formerly, my jacobparis.com website was in an Nx Monorepo with several other applications, but I can't leak the code for those so it was time to split it out somewhere I can share it properly. 

Why not just make it public?
- I rewrite the thing **a lot**. This website is more of a sandbox for me to try new things. I've rewritten my routing system twice already and it'll take at least one more before I'm happy with it.
- I want a clear separation between things I'm trying out and things I'm recommending. Doing things "the way jacob does it" by looking at my sandbox code is a recipe for disaster, and I have a reputation to uphold. 
- I'm willing to put more effort into answering questions and helping people 1:1 if think they'll stick around.

This is all very early stages, so expect a lot of changes 

## Remix Image Upload Example

This is an example replicating Slack's message input in Remix. 
- You can drag and drop images, or upload them, onto the message input.
- They show immediately in a pending "upload" state while they're uploaded in the background to the cloud. 
- Once the upload completes, they're replaced with the uploaded image and can be submitted with your form.

The draft message and any images in it is fully persisted to the server, so you can start a message on one device and finish it on another.

- Main blog post: https://www.jacobparis.com/content/remix-image-uploads
- Demo video: https://www.youtube.com/embed/Y-k1XXRtplk
- Example in code: https://github.com/jacobparis-insiders/jacobparis.com/tree/main/app/examples/remix-image-uploads

[![Optimistic Image Uploads In Remix](https://img.youtube.com/vi/Y-k1XXRtplk/0.jpg)](https://www.youtube.com/watch?v=Y-k1XXRtplk "Optimistic Image Uploads In Remix")

## Multi-step form demo with animated route transitions example

This is an example demonstrating forms that cross many pages, inspired by Linear's onboarding
- Data is submitted at every step to a form session object
- Users can navigate forward and backward through the form
- Users can jump to pages in the form out of order
- The server can infer, based on data in form session, whether a user should be allowed to access a certain page, and redirect them to the appropriate route if not

Each page loads with animated route transitions

- Main blog post: https://www.jacobparis.com/content/remix-multi-step-forms
- Animated route transitions blog post: https://www.jacobparis.com/content/remix-animated-page-transitions
- Demo video: https://www.youtube.com/embed/ck1cYiRP9Fw
- Example in code: https://github.com/jacobparis-insiders/jacobparis.com/tree/main/app/examples/remix-multi-step-forms

[![Multi-step form demo with animated route transitions](https://img.youtube.com/vi/ck1cYiRP9Fw/0.jpg)](https://www.youtube.com/watch?v=ck1cYiRP9Fw "Multi-step form demo with animated route transitions")

## Show active user presence (like Google Docs or Figma) example

This example covers how to show a presence indicator with a list of the users who are currently viewing a page

- Create a form with an emoji picker
- Use a cookie session storage to save the user's name and emoji.
- Create a full stack component to control the presence widget.
- Use event streams to update the presence widget in real time.

Websockets are also a viable solution here, but that requires setting up a separate websocket server. Server-sent events are easy and widely supported. 

- Main blog post: https://www.jacobparis.com/content/remix-presence
- Demo video: https://www.youtube.com/embed/WY1x91Ld-uw
- Example in code: https://github.com/jacobparis-insiders/jacobparis.com/tree/main/app/examples/remix-presence

[![Show active user presence (like Google Docs or Figma)](https://img.youtube.com/vi/WY1x91Ld-uw/0.jpg)](https://www.youtube.com/watch?v=WY1x91Ld-uw "Show active user presence (like Google Docs or Figma)")

## Autosave form inputs on change or blur example

This is an example demonstrating forms that persist automatically
- They useFetcher instead of submit so changes aren't lost on navigation

TODO: update to use the [useDebounceFetcher](https://www.jacobparis.com/content/use-debounce-fetcher) hook 
TODO: Add landing page + Get started button to create a custom ID so users changes don't conflict

- Main blog post: https://www.jacobparis.com/content/remix-form-autosave
- Example in code: https://github.com/jacobparis-insiders/jacobparis.com/tree/main/app/examples/remix-form-autosave
