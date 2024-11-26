# Folder Structures in React Projects

Organizing files and directories within a React project is crucial for maintainability, scalability, and ease of navigation. This repo explores the general architecture and folder structures across different scales of React projects, providing clear demonstrations for each level.

In general we can structure our folders in three ways depending on the project size:

- *Grouping by "File Types"*
- *Grouping by "File Types" and Features*
- *Grouping by "File Types" and Features*

> Please checkout to other three branches to get to know these folder structures.

## Give Consistent Meanings to Folder Names
Regardless of the structure level, certain folder names should carry specific meanings. What a folder name means may vary based on your preferences or the project's conventions.

Here's what I usually think about folder names:

### UI Components

- **components**: React components - the main UI building blocks.
- **design-system**: Fundamental UI elements and patterns based on the design system.
- **icons**: SVG icons that are meant to be used inline.

### React Specific

- **hooks**: Custom React hooks for shared logic.
- **hocs**: React Higher-order Components.
- **contexts/providers**: Contains React Contexts and Providers.

### Utilities & External Integrations

- **utils**: Utilities for universal logic that is not related to business logic or any technologies, e.g. string manipulations, mathematic calculations, etc.
- **lib**: Utilities that are related to certain technologies, e.g. DOM manipulations, HTML-related logic, localStorage, IndexedDB, etc.
- **plugins**: Third-party plugins (e.g. i18n, Sentry, etc.)

### Business Logic

- **services**: Encapsulates main business & application logic.
- **helpers**: Provides business-specific utilities.

### Styles

- **styles**: Contains (global) CSS or CSS-in-JS styles.

### TypeScript and Configurations

- **types**: For general TypeScript types, enums and interfaces.
- **configs**: Configs for the application (e.g. environment variables)
- **constants**: Constant, unchanged values (e.g. export const MINUTES_PER_HOUR = 60).

### Server Communication

- **api**: For logic that communicates with the server(s).
- **graphql**: GraphQL-specific code.

### State Management

- **states/store**: Global state management logic (Zustand, Valtio, Jotai, etc.)
- **reducers, store, actions, selectors**: Redux-specific logic

### Routing

- **routes/router**: Defining routes (if you're using React Router or the like).
- **pages**: Defining entry-point components for pages.

### Testing

- **tests**: Unit tests and other kinds of tests for your code.

## 🏁 Conclusion

Choosing the right folder structure in React projects is essential and should be based on the project's size and complexity. While "Level 1" may suffice for small projects, "Level 2" and "Level 3" offer more organized and modular structures for medium and large projects. Personally, I'd often recommend the "Level 2" folder structure. Also, Understanding common folder names helps maintain a consistent and intuitive architecture across React applications.

---

## Use this template for your project

```bash
npx create-ashk-app <project-name> --template simple
```

## Credits

- Inspired by these two articles [Folder Structures in React Projects](https://dev.to/itswillt/folder-structures-in-react-projects-3dp8) and [React Folder Structure in 5 Steps](https://www.robinwieruch.de/react-folder-structure/)
- The webpack.config.js file is seamlessly made with [createapp.dev](https://createapp.dev/)