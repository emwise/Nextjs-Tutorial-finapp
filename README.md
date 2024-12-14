## Next.js App Router Course - Starter

This is the starter template for the Next.js App Router Course. It contains the starting code for the dashboard application.

For more information, see the [course curriculum](https://nextjs.org/learn) on the Next.js Website.

## Notes

/app: Contains all the routes, components, and logic for your application, this is where you'll be mostly working from.
/app/lib: Contains functions used in your application, such as reusable utility functions and data fetching functions.
/app/ui: Contains all the UI components for your application, such as cards, tables, and forms. To save time, we've pre-styled these components for you.
/public: Contains all the static assets for your application, such as images.
Config Files: You'll also notice config files such as next.config.js at the root of your application. Most of these files are created and pre-configured when you start a new project using create-next-app. You will not need to modify them in this course.

    ## CSS

    You can start a project with Tailwind already installed and connected. You can also add custom CSS modules yourself. These allow you to create locally scoped styles to components by default, and will reduce the risk of styling conflicts. In this example the file app/ui/home.module.css provides a class that's locally applied to a div in app/page.tsx

    the clsx library can help you conditionally style elements of the page:
     
    import clsx from 'clsx';
 
    export default function InvoiceStatus({ status }: { status: string }) {
    return (
        <span
        className={clsx(
            'inline-flex items-center rounded-full px-2 py-1 text-sm',
            {
            'bg-gray-100 text-gray-500': status === 'pending',
            'bg-green-500 text-white': status === 'paid',
            },
        )}
        >
        // ...
    )}

## How to run the files

pnpm i #installs the dependancies 
pnpm dev starts running the files in http://localhost:3000