## Hi there 👋

This org is for all of my websites, code examples, and open source projects.

Previously, it was locked to newsletter subscribers only, but now everything is publicly available.

## Get in touch

I spend most of my life on [Twitter](https://twitter.com/jacobmparis) and the rest of it in [the Remix Discord](https://remix.run/docs/en/main/pages/community#discord).

## Remix Image Upload Example (like Slack)

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

## Show toast notifications on form submit with Remix

This is an example demonstrating how to show a toast message after a form is submitted.

- Main blog post: https://www.jacobparis.com/content/remix-form-toast
- Live example: https://www.jacobparis.com/content/remix-form-toast/example
- Example in code: https://github.com/jacobparis-insiders/jacobparis.com/tree/main/app/examples/remix-form-toast
- Demo video: https://www.youtube.com/embed/3IUYtO6QbbU

[![Show toast notifications on form submit with Remix](https://img.youtube.com/vi/3IUYtO6QbbU/0.jpg)](https://www.youtube.com/watch?v=3IUYtO6QbbU "Show toast notifications on form submit with Remix")

## Building a markdown input with a preview tab (like GitHub and Stack Overflow)

This is an example replicating GitHub's markdown preview input in Remix

- You can type markdown in the left pane and see the preview in the right pane.

- Main blog post: https://www.jacobparis.com/content/remix-markdown-preview
- Live example: https://www.jacobparis.com/content/remix-markdown-preview/example
- Example in code: https://github.com/jacobparis-insiders/jacobparis.com/tree/main/app/examples/remix-markdown-preview
- Demo video: https://www.youtube.com/embed/uK6cv_lzQwk

[![Building a markdown input with a preview tab](https://img.youtube.com/vi/uK6cv_lzQwk/0.jpg)](https://www.youtube.com/watch?v=uK6cv_lzQwk "Building a markdown input with a preview tab")


## Autosave form inputs on change or blur example

This is an example demonstrating forms that persist automatically
- useFetcher instead of submit so changes aren't lost on navigation

TODO: update to use the [useDebounceFetcher](https://www.jacobparis.com/content/use-debounce-fetcher) hook 
TODO: Add landing page + Get started button to create a custom ID so users changes don't conflict

- Main blog post: https://www.jacobparis.com/content/remix-form-autosave
- Live example: https://www.jacobparis.com/content/remix-form-autosave/example
- Example in code: https://github.com/jacobparis-insiders/jacobparis.com/tree/main/app/examples/remix-form-autosave

## Stream BullMQ Job Progress

This is an example of streaming progress updates for a pending BullMQ job
- BullMQ guide: https://www.jacobparis.com/content/bullmq-integration-guide
- Waiting for the job to complete: https://www.jacobparis.com/content/remix-defer-bullmq-queue
- Streaming the job's progress: https://www.jacobparis.com/content/remix-stream-bullmq-queue
- Example in code: https://github.com/jacobparis-insiders/remix-defer-streaming-bullmq

## Stream Progress Updates

This is a simpler example of streaming progress for a long-running task (no Redis or BullMQ)

- Main blog post: https://www.jacobparis.com/content/remix-defer-streaming-progress
- Example in code: https://github.com/jacobparis-insiders/remix-defer-streaming-progress
