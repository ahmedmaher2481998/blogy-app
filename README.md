

# Blogy - Blogging Platform

![][ci] ![][views] ![][stars] ![][forks] ![][issues] ![][license] ![][repo-size]


<!-- logo/title -->

<picture>
  <source media="(prefers-color-scheme: dark, (max-width:300px))" srcset="./public/logo-white.svg">
  <source media="(prefers-color-scheme: light,(max-width:300px))" srcset="./public/logo.svg">
  <img src="./public/logo-white.svg" width="300px" alt="Blogy Logo">
</picture>

 This is a feature-rich blogging platform built with Vue 3, using chadcn-vue, Supabase, and TypeScript.

<!-- <picture>
  <source media="(prefers-color-scheme: light)" srcset="https://graph.org/file/12ea4beff2367f40f13ce.png">
  <source media="(prefers-color-scheme: dark)" srcset="https://graph.org/file/16937ebb693470d804f31.png">
  <img src="https://graph.org/file/12ea4beff2367f40f13ce.png" alt="infinitunes">
</picture> -->

**[<kbd> <br> &nbsp;**Live Demo**&nbsp; <br> </kbd>][site]**

## Features

- User authentication with Google login
- Create, read, update, and delete blog posts
- Markdown support for writing blog posts
- View tracking for blog posts
- Tag management for blog posts
- User profiles
- Dark mode support
- File storage using Supabase Storage
- Transaction-like operations using PostgreSQL functions

## Technology Stack

- Vue 3
- TypeScript
- Supabase for backend, authentication, and file storage
- PostgreSQL functions for complex database operations
- chadcn-vue for UI components
- Markdown parser for blog post content
- Vitest for unit testing
- Vue Test Utils for component testing

## Getting Started

1. Clone the repository
2. Install dependencies: 
  ```sh
  pnpm install
  ```
3. Set up your Supabase project and add the credentials to your environment variables
4. Set up Supabase Storage buckets for file uploads
5. Create necessary PostgreSQL functions in your Supabase project
6. Run the development server: 
```sh 
pnpm run dev
```


## Testing

This project uses Vitest for unit testing and Vue Test Utils for component testing.

To run unit tests:
```sh
pnpm run test:unit
```

To run tests with coverage:
```sh
pnpm run test:unit:coverage
```

To run E2E tests:
```sh 
pnpm run test:e2e
```

## Project Structure

- `src/components`: Vue components
- `src/stores`: Pinia stores for state management
- `src/composables`: Reusable Vue composition functions
- `src/router`: Vue Router configuration
- `.spec.ts`: Test files
- `cypress` : E2E tests

## Key Components to Tested

1. Authentication components (e.g., LoginWithGoogle)
2. Blog post components (CreateBlogForms, MediaUpload)
3. Tag management components
4. User profile components
5. Navigation components
   <!-- 6. Comment system components adding -->
   <!-- 7. Search functionality adding -->
   <!-- 8. Pagination component adding -->
6. Rich text editor component


## Star History

<a href="https://star-history.com/#ahmedmaher2481998/blogy-app">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=ahmedmaher2481998/blogy-app&theme=dark" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=ahmedmaher2481998/blogy-app" />
   <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=ahmedmaher2481998/blogy-app" />
 </picture>
</a>
## Contributors:

[![][contributors]][contributors-graph]

_Note: It may take up to 24h for the [contrib.rocks][contrib-rocks] plugin to update because it's refreshed once a day._




## License

This project is licensed under the [MIT License] - see the [LICENSE.md](./License) file for details.




<!----------------------------------{ Labels }--------------------------------->

[views]: https://komarev.com/ghpvc/?username=blogy-app&label=view%20counter&color=red&style=flat
[repo-size]: https://img.shields.io/github/repo-size/ahmedmaher2481998/blogy-app
[issues]: https://img.shields.io/github/issues-raw/ahmedmaher2481998/blogy-app
[license]: https://img.shields.io/github/license/ahmedmaher2481998/blogy-app
[forks]: https://img.shields.io/github/forks/ahmedmaher2481998/blogy-app?style=flat
[stars]: https://img.shields.io/github/stars/ahmedmaher2481998/blogy-app
[contributors]: https://contrib.rocks/image?repo=ahmedmaher2481998/blogy-app&max=500
[contributors-graph]: https://github.com/ahmedmaher2481998/blogy-app/graphs/contributors
[contrib-rocks]: https://contrib.rocks/preview?repo=ahmedmaher2481998%2blogy-app
[ci]: https://github.com/ahmedmaher2481998/blogy-app/actions/workflows/ci.yml/badge.svg

<!-----------------------------------{ Links }---------------------------------->

[site]: https://blogy.vercel.app
