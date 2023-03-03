# Calculate-Price-for-WordPress-products
Tasks:

1. Register custom post types and custom taxonomy.
2. Create a Gutenberg block.
3. Implement logic when posting in one custom post type.

KEY STAGES
- Register custom post types
- You need to register 2 custom post types: “Products” and “Sets”.
- Register custom taxonomy
- You need to register 1 custom taxonomy “Brands”, which is linked to both post types
created in the previous step.
- Gutenberg block
- You need to register 1 gutenberg block for post types. With one input value
the cost of goods and kit.
- Product Publication
- When publishing a post in custom post type “Products”, it should be automatically published
post in custom post type “Sets” according to the following logic:
- This post in “Products” is not the only one in the linked taxonomy section
"Brands", if so, then:
- a new post is created in the post type “Sets”, which is attached to
the same heading taxonomy "Brands".
- the cost of all goods in this category is summed up and transferred from
discount -20%.
- new post title template “Set {category name}”.
- new post content template:
“This set includes:
{the ul list lists the title of the posts associated with this category}”
