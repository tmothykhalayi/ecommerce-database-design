Table product {
  product_id INT [pk, increment]
  product_name VARCHAR(255) [not null]
  brand_id INT [ref: > brand.brand_id]
  category_id INT [ref: > product_category.category_id]
  base_price DECIMAL(10,2) [not null]
}

Table product_image {
  image_id INT [pk, increment]
  product_id INT [ref: > product.product_id]
  image_url VARCHAR(255) [not null]
}

Table product_category {
  category_id INT [pk, increment]
  category_name VARCHAR(255) [not null]
}

Table color {
  color_id INT [pk, increment]
  color_name VARCHAR(100) [not null]
}

Table brand {
  brand_id INT [pk, increment]
  brand_name VARCHAR(255) [not null]
}

Table product_item {
  product_item_id INT [pk, increment]
  product_id INT [ref: > product.product_id]
  product_variation_id INT [ref: > product_variation.product_variation_id]
  price DECIMAL(10,2)
}

Table product_variation {
  product_variation_id INT [pk, increment]
  product_id INT [ref: > product.product_id]
  color_id INT [ref: > color.color_id]
  size_option_id INT [ref: > size_option.size_option_id]
}

Table size_category {
  size_category_id INT [pk, increment]
  size_category_name VARCHAR(100) [not null]
}

Table size_option {
  size_option_id INT [pk, increment]
  size_category_id INT [ref: > size_category.size_category_id]
  size_name VARCHAR(50) [not null]
}

Table product_attribute {
  attribute_id INT [pk, increment]
  product_id INT [ref: > product.product_id]
  attribute_type_id INT [ref: > attribute_type.attribute_type_id]
  attribute_value TEXT
}

Table attribute_category {
  attribute_category_id INT [pk, increment]
  attribute_category_name VARCHAR(255) [not null]
}

Table attribute_type {
  attribute_type_id INT [pk, increment]
  type_name VARCHAR(50) [not null]
}
