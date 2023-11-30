## Next.js App Router Course - Starter

This is the starter template for the Next.js App Router Course. It contains the starting code for the dashboard application.

For more information, see the [course curriculum](https://nextjs.org/learn) on the Next.js Website.

## "use client"

Client Component allowing the use event listeners and hooks.

## clsx:

Conditionally determine class names

## URLSearchParams

A Web API that provides utility methods for manipulating the URL query parameters.
Get the url params string e.g. _?page=1&query=a_.

**Use case**:
const num = searchParams.get(page) // returns '1'
const str = searchParams.get(query) // returns 'a'

## 'use server'

Mark all the exported functions within a file as server functions. Server functions can then be imported into Client and Server components.

## Folder structure

**app** - Root Segment
**dashboard** - Segment
**invoices** - Leaf Segment

**/app**: Contains all the routes, components, and logic for your application, this is where you'll be mostly working from.

**/app/lib**: Contains functions used in your application, such as reusable utility functions and data fetching functions.

**/app/ui**: Contains all the UI components for your application, such as cards, tables, and forms. To save time, we've pre-styled these components for you.

**/public**: Contains all the static assets for your application, such as images.

**/scripts**: Contains a seeding script that you'll use to populate your database in a later chapter.

**Config Files**: You'll also notice config files such as next.config.js at the root of your application. Most of these files are created and pre-configured when you start a new project using create-next-app. You will not need to modify them in this course.

### /(folderName)

Next.js uses a file-system based router where **folders** are used to define routes.

Each folder represents a **route segment** that maps to a **URL** segment.

A route group can be created by wrapping a folder's name in parenthesis (folderName).
'**()**' removes folder name from url path.
