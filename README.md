# SpiceGarden Restaurant Billing System

A modern, single-page restaurant billing application with menu management, cart billing, QR payment, and sales reporting.

## Features

- **Menu Management**: Add, edit, and delete menu items with images
- **Quick Billing**: Click menu items to add them directly to the cart
- **Cart Operations**: Adjust quantities, remove items, or clear the entire cart
- **Payment Flow**: Pay Now button displays QR code for payment confirmation
- **Bill Printing**: Print-friendly bill generation
- **Monthly Sales Report**: Track revenue, orders, and average ticket size by month
- **Search**: Quick search functionality to find menu items
- **Local Storage**: All data persists in browser localStorage (no backend required)

## Getting Started

1. Open `index.html` in a modern web browser
2. The app will initialize with default menu items: Idly, Dosa, Vada, Tea, Coffee, and Poori
3. Start using the app immediately - no installation required!

## Usage

### Adding Items to Bill
- Click any menu item card to add it to the cart
- Items are automatically added with quantity 1
- Click the same item again to increase quantity

### Managing Cart
- Use +/- buttons to adjust quantities
- Click × to remove an item from cart
- Click "Clear Cart" to remove all items

### Payment Process
1. Add items to cart
2. Click "Pay Now" button
3. QR code modal appears
4. Click "Confirm Payment" to finalize
5. Bill is automatically printed and cart is cleared

### Menu Management
1. Click "Manage Menu" button
2. View all current menu items
3. Click "Edit" on any item to modify it
4. Use the form to add new items or edit existing ones
5. Fill in: Name, Price, Category, and Image URL
6. Click "Save Item" to save changes
7. Click "Delete" to remove an item (only when editing)

### Sales Reports
- View monthly sales summary in the right panel
- Select different months from the dropdown
- See total revenue, order count, and average ticket size
- View detailed transaction history in the table below

### Printing Bills
- Click "Print Bill" to print the current cart as a bill
- Or complete payment to automatically print the finalized bill
- The print view is optimized for receipt printing

## Technical Details

- **Frontend**: Pure HTML, CSS, and JavaScript (ES6 modules)
- **Storage**: Browser localStorage
- **No Backend**: Fully client-side application
- **Responsive**: Works on desktop and mobile devices

## Browser Support

Works in all modern browsers that support:
- ES6 modules
- localStorage API
- CSS Grid and Flexbox

## Data Structure

- Menu items stored in `localStorage` with key `sg_menu_v1`
- Sales data stored with key `sg_sales_v1`
- Cart data stored with key `sg_cart_v1`

## Notes

- All data is stored locally in your browser
- Clearing browser data will reset the application
- For production use, consider backing up data regularly

