---
title: 'Add Reading Time Estimates to Your Next.js Blog'
description: 'Learn how to add a reading time estimate to your 
Next.js blog posts.'
date: '2023-11-29'
modified: '2023-12-08'
tags: ['nextjs','blog','webdev','opensource']
cover_image: true
---

I always like seeing reading time estimates for blog articles before I click the link. You can see examples of this on [my Hashnode blog page](https://yesdavidgray.com/) and on [my Medium profile](https://medium.com/@davegray_86804). I wanted to add this feature to my personal blog built with Next.js, too. 

Here's how I did it: 

## 1. reading-duration 

I found an npm package named [`reading-duration`](https://www.npmjs.com/package/reading-duration) that does a great job of calculating this value based on _words per minute_ while ignoring HTML tags. This is especially helpful when working with MDX files.  

Add it to your Next.js project with:
```bash
npm i reading-duration
```

## 2. Understand the settings 

You pass in your content to the `readingDuration` function this package provides, but there are some optional settings, too. You can set the `wordsPerMinute` (defaults to 200), and if you want, you can set the returned value to include an emoji (which is an hourglass ⏳). 

```tsx
import readingDuration from 'reading-duration'

const readingTime = readingDuration(rawMDXContent, {
  wordsPerMinute: 100, 
  emoji: false,
})
```

## 3. Add reading-duration to Your Next.js Blog

I store my MDX blog article files on GitHub and fetch them as my Next.js blog builds static pages. Below is an abbreviated version of what is happening in my code: 

```tsx
export async function getPostByName(fileName: string) {
    const res = await fetch(`my-github-url/${fileName}`)

    const rawMDX = await res.text()

    const duration = readingDuration(rawMDX, {
        emoji: false,
    })
}
```
I save the above `duration` value with the other `front matter` for the blog post. You can see I went with the default `wordsPerMinute` and declined the default emoji. When I use the duration value, I use an open book 📖 emoji instead.

You can see this value on [my blog homepage](https://www.davegray.codes/) for each article and near the top of each blog article page, too.

## 4. Open Source Update!

I thought it would be a nice addition to the [`reading-duration`](https://www.npmjs.com/package/reading-duration) package if we could have more emoji options built-in. _I submitted a pull request on GitHub with my suggested update_. I just received a reply from the author, and it looks like the update will be merged. 

With the update you can provide a `boolean | string` data type for the emoji option value. The boolean values work as shown above. The new string values provide different emojis in the output string. 

Here's a quick look at all possible emoji option values after the update:

```txt
true: '⌛ '
false: no emoji
hourglass_done: '⌛ '
hourglass_not_done: '⏳ '
stopwatch: '⏱ '
clock: '🕒 '
watch: '⌚ '
timer: '⏲ '
alarm: '⏰ '
books: '📚 '
open_book: '📖 '
closed_book: '📕 '
blue_book: '📘 '
green_book: '📗 '
orange_book: '📙 '
notebook: '📓 '
notebook_alt: '📔 '
```
