
General

    Creator_id  references
    Modified_by references


User
    
    first_name  string
    middle_name string
    last_name   string
    email       string
    active      boolean
    seller      boolean



Phone_number
    
    user_id     references
    number      string
    active      boolean


Address

    user_id             references
    street              string
    block               string
    lot                 string
    colony              string
    postal_code         string
    city                string
    state               string


flavour

    name                string
    active              string

condition

    name                string
    active              string


product_class

    name                string
    active              boolean


Single

    product_class_id    references
    name                string
    flavour             references     
    condition           references
    tumbnail            attachment

selling product


shopping_cart

    product_id          references


