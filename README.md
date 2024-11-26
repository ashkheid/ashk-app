# Level 3: Grouping by Features/Modules

For larger projects, the "Level 3" structure offers a highly modular approach, defining clear boundaries for different aspects of the application within each module:

```
└── src/
    ├── assets/
    ├── modules/
    |   ├── core/
    │   │   ├── components/
    │   │   ├── design-system/
    │   │   │   └── Button.tsx
    │   │   ├── hooks/
    │   │   ├── lib/
    │   │   └── utils/
    │   ├── payment/
    │   │   ├── components/
    │   │   │   └── PaymentForm.tsx
    │   │   ├── hooks/
    │   │   │   └── usePayment.ts
    │   │   ├── lib/
    │   │   ├── services/
    │   │   ├── states/
    │   │   └── utils/
    │   ├── auth/
    │   │   ├── components/
    │   │   │   └── SignUpForm.tsx
    │   │   ├── hooks/
    │   │   │   └── useAuth.ts
    │   │   ├── lib/
    │   │   ├── services/
    │   │   ├── states/
    │   │   └── utils/
    │   └── employees/
    │       ├── components/
    │       │   ├── EmployeeList.tsx
    │       │   └── EmployeeSummary.tsx
    │       ├── hooks/
    │       │   ├── useEmployees.ts
    │       │   └── useUpdateEmployee.ts
    │       ├── services/
    │       ├── states/
    │       └── utils/
    └── ...
```

- **Project Size**: Large and Complex
- **Advantages**:
  - Stuff are clearly grouped by features/modules
  - Features/Modules are clear representations of objects in the real world
- **Disadvantages**:
  - You'll have to be well-aware of the business logic to make the right grouping decisions

With this, if you are to remove or modify the payment logic, you'll know right away where to start.

---

## Use this template for your project

```bash
npx create-ashk-app <project-name> --template by-file-and-feature
```

## Credits

- Inspired by these two articles [Folder Structures in React Projects](https://dev.to/itswillt/folder-structures-in-react-projects-3dp8) and [React Folder Structure in 5 Steps](https://www.robinwieruch.de/react-folder-structure/)
- The webpack.config.js file is seamlessly made with [createapp.dev](https://createapp.dev/)