# Custom Fields on Order

Since v2.2.1 you can add custom-defined fields to the order form.

## Setting up the custom fields <a id="setting-up-the-custom-fields"></a>

The custom fields can be entered if you login as admin and then go to Site Setting. There go to the "Setup" tab and on the bottom, you will see the "Custom fields" section.

The custom fields are defined using JSON syntax. So make sure [you have a valid](https://jsonlint.com/) JSON string.

Here is an example of custom fields. You can use this [tool](https://jsoneditoronline.org/) to create the JSON.

```text
[{        "title": "Customer phone numner",        "key": "customer_phone_number",        "ftype": "input",        "type": "phone",        "placeholder": "Enter your phone"    },    {        "title": "Customer email",        "key": "customer_email",        "ftype": "input",        "type": "email",    },    {        "title": "Country",        "key": "customer_country",        "ftype": "select",        "data": {            "macedonia": "Macedonia",            "usa": "United States of America"        }    },    {        "title": "is this a gift",        "key": "send_as_gift",        "ftype": "bool",        "value": true    },    {        "title": "Custom note",        "key": "custom_note",        "ftype": "textarea"    }]
```

In the example above, this will output 5 form fields in the order tab.

![](https://i.imgur.com/WWMyFgq.png)

Custom Fields

Here is an explanation of the different fields use

## Translation of the custom fields <a id="translation-of-the-custom-fields"></a>

You should add translation keys for these custom fields keys inside the translation menu. Add them to the "**custom**" group as shown on the image.

![](https://i.imgur.com/hKNpl8J.png)

Add new language

