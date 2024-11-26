# ⭐ Level 2: Grouping by "File Types" and Features

As projects grow, the "Level 2" structure introduces grouping by feature within each type:

```
└── src/
    ├── assets/
    ├── api/
    ├── configs/
    ├── components/
    │   ├── auth/
    │   │   └── SignUpForm.tsx
    │   ├── payment/
    │   │   └── PaymentForm.tsx
    │   ├── common/
    │   │   └── Button.tsx
    │   └── employees/
    │       ├── EmployeeList.tsx
    │       └── EmployeeSummary.tsx
    ├── hooks/
    │   ├── auth/
    │   │   └── useAuth.ts
    │   ├── payment/
    │   │   └── usePayment.ts
    │   └── employees/
    │       ├── useEmployees.ts
    │       └── useUpdateEmployee.ts
    ├── lib/
    ├── services/
    ├── states/
    └── utils/
```

- **Project Size**: Medium to Large
- **Advantages**:
  - Simple & straightforward
  - Stuff are grouped by features
- **Disadvantages**:
  - Logic related to a feature is still spread across multiple folder types

Now let's come back to the problem statement where the payment module needs to be modified or removed. With this structure, it's a lot easier to do that now.

> ⭐ The "Level 2" folder structure is the one that I'd recommend if you don't know what to choose.

---

## Use this template for your project

```bash
npx create-ashk-app <project-name> --template by-file-and-feature
```

## Credits

- Inspired by these two articles [Folder Structures in React Projects](https://dev.to/itswillt/folder-structures-in-react-projects-3dp8) and [React Folder Structure in 5 Steps](https://www.robinwieruch.de/react-folder-structure/)
- The webpack.config.js file is seamlessly made with [createapp.dev](https://createapp.dev/)