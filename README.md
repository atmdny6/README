# Project Structure

```text
AuthKitty/
├── assets/                                           # Static assets (icons)
│
├── src/                                              # Main source code
│   ├── auth/                                         # Authentication
│   │   ├── components/                               # Authentication related layouts/components
│   │   │   └── AuthLayout.tsx                        # Authentication page layout
│   │   │
│   │   ├── hooks/                                    # Authentication hooks
│   │   │   └── useAuth.ts                            # Authentication state & logic
│   │   │
│   │   └── modals/                                   # Authentication screens
│   │       ├── SignIn.tsx                            # User sign-up page
│   │       └── SignUp.tsx                            # User sign-in page
│   │
│   ├── dash/                                         # Dashboard
│   │   ├── components/                               # Dashboard layouts
│   │   │   ├── DashboardLayout.tsx                   # Main dashboard layout
│   │   │   └── DrawerLayout.tsx                      # Sidebar Settings drawer layout
│   │   │
│   │   ├── hooks/                                    # Dashboard hooks
│   │   │   ├── useAccounts.ts                        # Account management hook
│   │   │   └── useSettings.ts                        # Settings management hook
│   │   │
│   │   ├── modals/                                   # Dashboard modal dialogs
│   │   │   ├── AccountAddModal.tsx                   # Add account modal
│   │   │   ├── AccountEditModal.tsx                  # Edit account modal
│   │   │   ├── AccountDeleteModal.tsx                # Delete account confirmation modal
│   │   │   ├── AccountAlertModal.tsx                 # Alert account modal (worning, errors, alerts etc)
│   │   │   └── AccountSettingsModal.tsx              # Account all settings drawer modal
│   │   │
│   │   └── ui/                                       # Reusable dashboard UI
│   │       ├── AccountCard.tsx                       # Account card component
│   │       ├── AccountIcon.tsx                       # Account icon component
│   │       ├── CircularProgress.tsx                  # Loading progress indicator
│   │       └── ToastContainer.tsx                    # ToastContainer component
│   │
│   ├── hooks/                                        # Global custom hooks
│   │   ├── useToast.ts                               # Toast hook
│   │   └── useTotp.ts                                # TOTP generation hook
│   │
│   ├── types/                                        # TypeScript type definitions
│   │   └── index.ts                                  # Shared interfaces & types
│   │
│   ├── utils/                                        # Utility/helper functions
│   │   ├── domains.ts                                # Domain-related helpers
│   │   └── importExport.ts                           # Import/export utilities
│   │
│   ├── App.tsx                                       # Root React component
│   ├── background.ts                                # Chrome extension background script
│   ├── sidepanel.tsx                                # Extension side panel entry
│   ├── preloader.ts                                 # Preload script
│   └── index.css                                    # Global styles
│
├── .env.chrome.example                              # Chrome extension env template
├── .env.development.example                         # Development env template
├── .env.production.example                          # Production env template
├── .gitignore                                       # Git ignored files
├── .prettierrc.cjs                                  # Prettier configuration
├── README.md                                        # Project documentation
├── package.json                                     # Dependencies & scripts
└── tsconfig.json                                    # TypeScript configuration
```
