# Project Structure

```text
AuthKitty/
├── assets/                                            # Static assets (icons, images, fonts)
│
├── src/                                               # Main source code
│   ├── auth/                                          # Authentication module
│   │   ├── components/                               # Auth-related layouts/components
│   │   │   └── AuthLayout.tsx                        # Authentication page layout
│   │   │
│   │   ├── hooks/                                    # Auth custom hooks
│   │   │   └── useAuth.ts                            # Authentication state & logic
│   │   │
│   │   └── modals/                                   # Authentication screens/modals
│   │       ├── SignIn.tsx                            # User sign-in page
│   │       └── SignUp.tsx                            # User registration page
│   │
│   ├── dash/                                         # Dashboard module
│   │   ├── components/                               # Dashboard layouts
│   │   │   ├── DashboardLayout.tsx                   # Main dashboard layout
│   │   │   └── DrawerLayout.tsx                      # Sidebar drawer layout
│   │   │
│   │   ├── hooks/                                    # Dashboard hooks
│   │   │   ├── useAccounts.ts                        # Account management hook
│   │   │   └── useSettings.ts                        # Settings management hook
│   │   │
│   │   ├── modals/                                   # Dashboard modal dialogs
│   │   │   ├── AccountAddModal.tsx                   # Add account modal
│   │   │   ├── AccountEditModal.tsx                  # Edit account modal
│   │   │   ├── AccountDeleteModal.tsx                # Delete account confirmation
│   │   │   ├── AccountAlertModal.tsx                 # Alert modal
│   │   │   └── AccountSettingsModal.tsx              # Account settings modal
│   │   │
│   │   └── ui/                                       # Reusable dashboard UI
│   │       ├── AccountCard.tsx                       # Account card component
│   │       ├── AccountIcon.tsx                       # Account icon component
│   │       ├── CircularProgress.tsx                  # Loading progress indicator
│   │       └── ToastContainer.tsx                    # Notification container
│   │
│   ├── hooks/                                        # Global custom hooks
│   │   ├── useToast.ts                               # Toast notification hook
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
