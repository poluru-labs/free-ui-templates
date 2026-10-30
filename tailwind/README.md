# Free Web & Mobile Templates (Tailwind)

**Repository:** [github.com/poluru-labs/subrahmanyam-poluru-free-web-mobile-templates](https://github.com/poluru-labs/subrahmanyam-poluru-free-web-mobile-templates)

Responsive **Tailwind CSS** website and dashboard templates under `web/tailwind/`. Most folders are **static HTML** using the **Tailwind v4 browser build** (`@tailwindcss/browser`), **Bootstrap Icons**, and **Google Fonts** (Roboto, Lato, Open Sans on newer demos)—**no install step**. **Whitmore Academy** (`school-parent-dashboard`) is a **React + Vite** app.

Part of the [Free UI Templates](../README.md) catalog. Bootstrap templates in the same repository are listed in [../bootstrap/README.md](../bootstrap/README.md).

## Available templates

**49** Tailwind demos (folder names below are relative to `web/tailwind/`).

| Product | Use case | Folder |
| --- | --- | --- |
| Threadline | AI chat workspace | `ai-chat-workspace` |
| Gridline | Analytics & BI dashboard | `analytics-saas-dashboard` |
| Subbu Balance | Budget planner dashboard | `budget-planner-dashboard` |
| Keyline | Car rental marketplace | `car-rental-marketplace` |
| Stackforge | Coding bootcamp landing | `coding-bootcamp-landing` |
| Commonroom | Community discussion forum | `community-discussion-forum` |
| Workbay | Coworking space booking | `coworking-space-booking` |
| Signaldesk | Customer feedback board | `customer-feedback-board` |
| CaseHarbor | Customer support helpdesk | `customer-support-helpdesk` |
| Poluru DevDocs | Developer documentation portal | `developer-documentation-portal` |
| Poluru Assets | Digital asset marketplace | `digital-asset-marketplace` |
| Poluru Seller | Ecommerce seller dashboard | `ecommerce-seller-dashboard` |
| Poluru Onboard | Employee onboarding portal | `employee-onboarding-portal` |
| Poluru Tickets | Event ticketing platform | `event-ticketing-platform` |
| Stride | Fitness coach dashboard | `fitness-coach-dashboard` |
| PlateHarbor | Food delivery app UI | `food-delivery-app-ui` |
| Subra Studio | Freelancer invoicing | `freelancer-invoicing` |
| StreakHarbor | Habit tracker app | `habit-tracker-app` |
| Poluru Care | Healthcare appointment portal | `healthcare-appointment-portal` |
| Poluru Home | Home services marketplace | `home-services-marketplace` |
| Poluru Claims | Insurance claims portal | `insurance-claims-portal` |
| Poluru Stock | Inventory management dashboard | `inventory-management-dashboard` |
| BillHarbor | Invoice generator SaaS | `invoice-generator-saas` |
| Folio | Job application tracker | `job-application-tracker` |
| Poluru Legal | Legal case management | `legal-case-management` |
| Poluru Track | Logistics shipment tracker | `logistics-shipment-tracker` |
| MealHarbor | Meal planner dashboard | `meal-planner-dashboard` |
| WaveHarbor | Music streaming UI | `music-streaming-ui` |
| Poluru Give | Nonprofit donation platform | `nonprofit-donation-platform` |
| BookHarbor | Online bookstore | `online-bookstore` |
| TrainHarbor | Personal trainer booking | `personal-trainer-booking` |
| Pawlane | Pet adoption platform | `pet-adoption-platform` |
| Poluru Cast | Podcast discovery app | `podcast-discovery-app` |
| Parkline | Property management portal | `property-management-portal` |
| Poluru Homes | Real estate listings | `real-estate-listings` |
| Simmerbox | Recipe sharing community | `recipe-sharing-community` |
| Poluru Table | Restaurant reservation app | `restaurant-reservation-app` |
| Whitmore Academy | School parent portal (**Vite + React**) | `school-parent-dashboard` |
| Poluru Plan | Social media content calendar | `social-media-content-calendar` |
| Quill | Student LMS portal | `student-lms-portal` |
| BoxHarbor | Subscription box storefront | `subscription-box-storefront` |
| Poluru Forms | Survey form builder | `survey-form-builder` |
| Ledger | Teacher gradebook | `teacher-gradebook` |
| Poluru Trips | Travel itinerary planner | `travel-itinerary-planner` |
| Harborwell | University admissions | `university-admissions` |
| Reeldesk | Video course marketplace | `video-course-marketplace` |
| Poluru Serve | Volunteer coordination platform | `volunteer-coordination-platform` |
| Poluru Depot | Warehouse operations dashboard | `warehouse-operations-dashboard` |
| Vowline | Wedding planner website | `wedding-planner-website` |

**Technologies:** HTML5, Tailwind CSS v4 (CDN browser build on static templates), JavaScript, Bootstrap Icons, Google Fonts. Demo interactivity often uses **localStorage** (saved items, forms, filters)—no live backend. Chart or calendar widgets where noted in each folder’s `README.md`.

## Getting started

Static templates (from repository root):

```bash
git clone https://github.com/poluru-labs/subrahmanyam-poluru-free-web-mobile-templates.git
cd subrahmanyam-poluru-free-web-mobile-templates
python3 -m http.server 8000
# Example: http://localhost:8000/web/tailwind/community-discussion-forum/
```

Whitmore Academy parent portal:

```bash
cd web/tailwind/school-parent-dashboard
npm install
npm run dev
```

Per-template preview ports and notes (when set) are in each folder’s `README.md`.

## Author

[Subrahmanyam Poluru](https://polurus.com) · mail.polurus@gmail.com
