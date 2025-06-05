import { createBrowserRouter, RouterProvider } from "react-router-dom";

const router = createBrowserRouter([
  {
    path: "/",
    element: <App />,
    errorElement: <CustomErrorElement />,
    children: [
      // child routes
    ],
  },
]);

function CustomErrorElement() {
  return (
    <div>
      <h1>Something went wrong!</h1>
      <p>Please check your connection or try again.</p>
    </div>
  );
}

<RouterProvider router={router} /> minikit-js

## 🚀 Getting Started

MiniKit is currently available on npm. To install, run:
`pnpm i @worldcoin/minikit-js`

or use the CDN:
`https://cdn.jsdelivr.net/npm/@worldcoin/minikit-js@[version]/+esm`

For comprehensive setup instructions and usage examples, visit our [developer documentation](https://docs.world.org/mini-apps).

## 🛠 ️Developing Locally

To run the example mini app locally:

```
pnpm i
cd demo/with-next
pnpm dev
```

This will launch a demo mini app with all essential commands implemented, allowing you to explore and test the features.

## 📦 Releasing

To bump the version of the package, run:

```
pnpm changeset
```
