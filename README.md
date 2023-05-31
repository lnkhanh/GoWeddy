<p align="center">
  <a href="https://goweddy.net">
    <img src="https://goweddy.net/assets/images/logo-black.png" width="314px" alt="GoWeddy logo" />
  </a>
</p>
<h3 align="center">Start mapping your lineage with our user-friendly family tree creator!</h3>
  
- [Try live demo](https://goweddy.net/login) (Account: john.doe@goweddy.net/GoWeddy@2023!)
- [Get the source code](https://kluong.gumroad.com/l/genealogy-tree) 

# Introduction

The Genealogy Tree is is developed using the Next.js framework and Strapi CMS. Next.js is a popular React framework that provides server-side rendering and static site generation capabilities, making it efficient for building fast and dynamic web applications. Strapi is a headless CMS that allows for easy content management and API creation.
  

By utilizing Next.js, the family tree website ensures a smooth and interactive user experience, with optimized performance and SEO-friendly features. The framework's server-side rendering capability enables the website to load quickly and provide immediate content to users.

Strapi CMS empowers administrators to manage and organize family tree data effortlessly. With its intuitive user interface, administrators can easily create, update, and delete family member information, relationships, and important notes. Strapi's powerful API creation enables seamless integration of the website with various front-end technologies.

The combination of Next.js and Strapi CMS provides a robust foundation for the family tree website, offering flexibility, scalability, and efficient content management. It allows users to explore their family history, connect with relatives, and share valuable information easily.

# Features
- **Create, Update, and Delete**: Users can easily create new family members, update their information, and delete existing entries. This allows for maintaining an accurate and up-to-date family tree.

- **Search Family Members**: The website provides a search functionality, enabling users to quickly find specific family members within their tree. This makes it easy to navigate and explore different branches of the family.

- **Login Options**: The website supports multiple login methods, including traditional username/password authentication, as well as social login options with **Google** and **Facebook** accounts. This provides users with flexibility and convenience when accessing their family tree.

- **Sign Up**: New users can register for an account on the website, allowing them to create and manage their own family tree. The sign-up process is user-friendly and ensures that each user has a personalized experience.

- **Forgot Password**: In case users forget their password, the website offers a password recovery feature. Users can initiate the password reset process by providing their registered email address and following the instructions sent to their inbox.

- **User Profile**: Each user has their own profile on the website, which allows them to view and manage their personal information, preferences, and settings. Users can update their profile details, such as their name, profile picture, and contact information, providing a personalized experience within the platform.

- **Admin Panel**: The admin panel is a dedicated section of the website accessible only to authorized administrators. From the admin panel, administrators have the ability to manage end users and assets. This includes functionalities like creating and editing user accounts, assigning roles and permissions, and overseeing the overall system configuration.

- **User Management**: Administrators can create new user accounts, deactivate or delete existing accounts, and modify user details. They can also assign specific roles and permissions to users based on their responsibilities or access level within the system.

- **Asset Management**: The admin panel allows administrators to manage assets related to the Family Tree website. This may include uploading and organizing files, such as documents, photos, or multimedia content, that are associated with the family tree or individual family members.

- **Auto-generating language files**: Language files contain translations for different languages used in your application.

- **Auto-generating environment file**: Environment file store configuration variables specific to different environments (e.g., development, production, staging).

# Installation


### Prerequisites:

- Make sure you have **Node.js 16 or later** installed on your system. You can download it from the official Node.js website (https://nodejs.org).

- Ensure you have a package manager installed, such as npm (comes with Node.js) or yarn (https://yarnpkg.com).

## Strapi CMS Administrator (https://docs.strapi.io/dev-docs/installation/cli)

  

Open your terminal or command prompt.

Install the Strapi CLI globally by running the following command:


```
npm install -g strapi
```
  
or

```
yarn global add strapi
```

Navigate into the unzipped directory:

```
cd <your_directory>/GenealogyTree/admin && npm install
```

Start the Strapi development server:


```
npm run develop
```

or

```
yarn develop
```

You should see output indicating that the Strapi server is running and listening for requests. Open your browser and access the Strapi admin panel by visiting http://localhost:1337/admin (Account: admin@goweddy.net/GoWeddy@2023!).

That's it! You have successfully installed Strapi CMS. You can now start building your content types, APIs, and managing your website's data through the Strapi admin panel.

Read this for setting up login providers on website: https://docs.strapi.io/dev-docs/plugins/users-permissions#providers

## Next.js (https://docs.strapi.io/dev-docs/installation/cli)

Navigate into the unzipped directory:

```
cd <your_directory>/GenealogyTree/app && npm install -f
```

Start the Next.js development server:

  

```
npm run dev
```

or

```
yarn dev
```

Next.js will compile your project and start the development server. You should see output indicating that the server is running and listening for requests.

Open your browser and access your Next.js application by visiting http://localhost:3000.

You can sign up or sign in with default user: john.doe@goweddy.net/GoWeddy@2023!

## Environments

Automation generates a **.env** file.

The Node.js automation project for generating environment configuration is designed to streamline the process of creating environment-specific configuration files for your Node.js applications. It provides a convenient way to automate the generation of environment-specific variables and settings, making it easier to manage different configurations for development, staging, and production environments.

By leveraging this automation project, you can avoid the manual effort of duplicating and modifying configuration files for each environment. Instead, you can define a template configuration file with placeholders for environment-specific values. Then, using a script or tool, you can generate the actual configuration files by replacing the placeholders with the appropriate values based on the target environment.

This automation process allows for efficient management of environment-specific settings, such as database credentials, API keys, external service URLs, and other variables that may differ across environments. It helps maintain consistency and reduces the risk of configuration errors when deploying your Node.js applications to different environments.

Overall, the Node.js automation project for generating environment config simplifies the task of managing environment-specific configuration files, enhances development productivity, and ensures accurate configuration across different deployment environments.

Navigate into the unzipped directory:

```
cd <your_directory>/GenealogyTree/environments && npm install
```

#### For Strapi CMS Administrator:
**Sign up for a Cloudinary account:** 
Visit the Cloudinary website (https://cloudinary.com) and sign up for a free account. Once you have created an account, you will have access to your Cloudinary cloud name, API key, and API secret. And update it to `<your_directory>/GenealogyTree/environments>/admin_configs/development.ts` file.

Generating...

Development environment:

```
npm run build.admin.dev
```

Production environment:

```
npm run build.admin.prod
```

#### For Next.js Application:

Development environment:

```
npm run app.admin.dev
```

Production environment:

```
npm run build.app.prod
```

### Multilingual

The Node.js automation project for multilingual configuration is designed to facilitate the management of multilingual content in your Node.js applications. It provides a convenient way to define and organize language-specific configuration files, allowing your application to dynamically load and display content in different languages based on user preferences or other criteria.

With this automation project, you can easily define separate configuration files for each supported language, containing language-specific variables, translations, or any other language-related settings.

Navigate into the unzipped directory:

```
cd <your_directory>/GenealogyTree/languages && npm install
```

and

```
npm run gen.en && npm run gen.vi
```

Please visit `<your_directory>/GenealogyTree/app/public/locales` to check the results.


### License

See the [LICENSE](./LICENSE) file for licensing information.
