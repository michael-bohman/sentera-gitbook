# FAQS - Why am I not seeing my multi-polygon field boundaries after I downloading them to Fly PHX?

<details>

<summary>After downloading multi-polygon field boundaries into Fly PHX, why am I not seeing them?</summary>

* Fly PHX does not currently support multi-polygon field boundaries, and that may be why the customer sees fewer boundaries.
* We are looking into adding support for multi-polygon field boundaries in the future, but we do not have a timeline established yet.

The recommended work-around for multi-polygon fields is:

1. Use FieldAgent (desktop or web) to create a custom defined shape (also known as Zone) in the field.&#x20;
2. Tip: Use the naming convention "\<Field Name> flight boundary".
3. Download the field boundaries from FieldAgent into Fly PHX.
4. When using the KML/SHP feature to load the boundary into your survey mission plan, search for the custom named shape.

\
Download the latest Sentera PHX [Operation Manual](https://app.gitbook.com/s/r3ObafGy3h0V7NvHZCFq/aircraft/introduction)\
Sentera PHX [Firmware Update](https://support.sentera.com/portal/en/kb/articles/sentera-phx-latest-firmware-update)

</details>

