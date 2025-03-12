You are a skilled WordPress developer tasked with creating a WooCommerce-supportive AI Chatbox plugin with the following functionalities:
1. **Frontend Chatbox**:
   - A visually appealing and responsive chatbox appears on the frontend of the WooCommerce-powered website.
   - Users (visitors and logged-in customers) can initiate and participate in chat conversations. If logged out user intiate the conversation System message will be different. and order status will not be send for logged out users.
- Make sure page caching not work when we get the user id and its orders.
   - AI responds to user queries based on a provided system message containing structured website-related information and standard responses.
-  Manage multiple response from AI
2. **Integration with WooCommerce**:
   - If a user is logged in, the system automatically retrieves and sends the user's last 20 orders, including:
     - Order IDs
     - Order statuses (e.g., pending, completed, shipped)
     - Custom meta-data from `wp_postmeta`, specifically:
       - Payment numbers: `woo_bkash_number`, `woo_nagad_number`, `woo_rocket_number`
       - Transaction IDs: `woo_bkash_trans_id`, `woo_nagad_trans_id`, `woo_rocket_trans_id`
3. **Backend Management**:
   - All conversations are logged and viewable within the WordPress admin dashboard.
   - Administrators or support staff can review conversation history.
   - Human support agents can seamlessly take over conversations from the AI at any point from the backend interface.
4. **AI Integration and Customization**:
   - The plugin uses a predefined system message to guide AI responses, ensuring relevance to the website's specific context.
   - The system message and related data/answers should be easily updatable by site administrators from the backend.
Write clean, maintainable, and secure code, following WordPress plugin development best practices and ensuring compatibility with WooCommerce.


Now write me the full plugin code with File structure
