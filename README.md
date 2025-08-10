<h1>Electronics eCommerce Shop With Admin Dashboard in Next.js and Node.js</h1>

<p>
  <b>eCommerce system with an admin dashboard built with Next.js and Node.js</b>
  is a personal project developed by <b>Angel Curtido</b>, a Systems Analysis graduate and
  full-stack developer. The application is coded from scratch with a custom design,
  fully responsive, and powered by MySQL. This project is part of my professional portfolio,
  showcasing my ability to design, implement, and deploy a modern online store that handles the
  entire purchase flow along with a comprehensive admin panel for managing products, orders, and users.
</p>

<h2>Instructions</h2>
<ol>
  <li>
    <p>
      Download and install Node.js (includes npm) from
      <a href="https://nodejs.org/en" target="_blank">https://nodejs.org/en</a>.
    </p>
  </li>

  <li>
    <p>
      Install MySQL locally. You can use the standalone installer from
      <a href="https://dev.mysql.com/downloads/installer/" target="_blank">
        https://dev.mysql.com/downloads/installer/
      </a>.
      <br />
      <em>Alternative:</em> you can also spin up MySQL (and Apache) with
      <b>XAMPP</b>; simply install XAMPP and enable the <i>Apache</i> and
      <i>MySQL</i> modules from its control panel.
    </p>
  </li>

  <li>
    <p>
      (Optional) Install a graphical database client such as
      <a href="https://www.heidisql.com" target="_blank">HeidiSQL</a> for easier
      data management.
    </p>
  </li>

  <li>
    <p>
      Clone or download this repository and extract it to your workspace.
    </p>
  </li>

  <li>
    <p>
      Open the project folder in your code editor and create a
      <code>.env</code> file at the root.
    </p>
  </li>

  <li>
    <p>
      Add the following environment variables to <code>.env</code>, replacing
      <code>username</code> and <code>password</code> with your MySQL
      credentials:
    </p>
    <!-- Example -->
    <!--
    DB_HOST=localhost
    DB_PORT=3306
    DB_USER=username
    DB_PASSWORD=password
    DB_NAME=ecommerce
    -->
  </li>
</ol>

```
DATABASE_URL="mysql://username:password@localhost:3306/ecommerce" 
NEXTAUTH_SECRET=12D16C923BA17672F89B18C1DB22A
NEXTAUTH_URL=http://localhost:3000
```

<p>7. After you do it, you need to create another .env file in the server folder and put the same DATABASE_URL you used in the previous .env file:</p>

```
DATABASE_URL="mysql://username:password@localhost:3306/ecommerce"
```

<p>8. Now you need to open your terminal of choice in the root folder of the project and write:</p>


```
npm install
```

<p>9. Now you need to navigate with the terminal in the server folder and install everything:</p>

```
cd server
npm install
```

<p>10. You will need to run the Prisma migration now. Make sure you are in the server folder and write:</p>

```
npx prisma migrate dev
```

<p>11. Next is to insert demo data. To do it you need to go to the server/utills folder and call insertDemoData.js:</p>

```
cd utills
node insertDemoData.js
```

<p>12. Now you can go back to the server folder and run the backend:</p>

```
cd ..
node app.js
```

<p>13. While your backend is running you need to open another terminal(don't stop the backend). In the second terminal, you need to make sure you are in your root project folder and write the following:</p>

```
npm run dev
```

<p>14. Open <a href="http://localhost:3000" target="_blank">http://localhost:3000</a> and see it live!</p>


<h2>Project screenshots</h2>

<h3>Home page</h3>
<img src="./assets/homepage1.PNG" alt="Ecommerce home page" width="800">
<h3>Shop page</h3>
<img src="./assets/shoppage1.PNG" alt="ShopPage" width="800">
<h3>Single product page</h3>
<img src="./assets/singleproductpage.PNG" alt="Single product page" width="800">
<h3>Register page</h3>
<img src="./assets/registerpage.PNG" alt="Register page" width="800">
<h3>Login page</h3>
<img src="./assets/loginpage.PNG" alt="Login page" width="800">
<h3>Search page</h3>
<img src="./assets/searchpage.PNG" alt="Search page" width="800">
<h3>Wishlist page</h3>
<img src="./assets/whitlistpage.PNG" alt="Wishlist page" width="800">
<h3>Cart page</h3>
<img src="./assets/cartpage.PNG" alt="Cart page" width="800">
<h3>Checkout page</h3>
<img src="./assets/checkoutpage.PNG" alt="Checkout page" width="800">
<h3>Admin dashboard - All orders page</h3>
<img src="./assets/admindashboardorderpage.PNG" alt="Admin dashboard - All orders page" width="800">
<h3>Admin dashboard - All products page</h3>
<img src="./assets/admindashboardproductpage.PNG" alt="Admin dashboard - All products page" width="800">
<h3>Admin dashboard - All categories page<h3>
<img src="./assets/admindashboardcategorypage.PNG" alt="Admin dashboard - All products page" width="800">
<h3>Admin dashboard - All users page</h3>
<img src="./assets/admindashboarduserpage.PNG" alt="Admin dashboard - All products page" width="800">