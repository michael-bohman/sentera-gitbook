# Pix4D - Adding Single Sensor Pix4D Templates (NDVI and NDRE)

The instructions and templates below will help you use **Pix4D (Version 4.5.2)** with your Sentera Single Sensor. Make sure to download the correct template for your sensor. Using the incorrect template will produce inaccurate results. If you are not sure what type of sensor you have, contact us at [support@sentera.com](mailto:support@sentera.com). We will need the model and serial number located on the label that is on the sensor.\
\
**If you have an older version of Pix4D with the "sentera\_single\_precision\_ndvi\_2018\_01\_22" or "sentera\_single\_precision\_ndre\_2018\_01-22" template please follow the instructions below.**

**Updating the Template for an older version of Pix4D to support the Single Sensor Firmware 2.3.2 or higher (Late January 2020).**

1\.     Run the project as you normally would with the old template.  When the project is done, click on Index Calculator.

<div align="left"><figure><img src="../../.gitbook/assets/Picture1.png" alt="" width="317"><figcaption></figcaption></figure></div>

2\.     Check to see if the NDVI and NDRE indices are present in the dropdown. If missing, click Indices and continue to Step 3.&#x20;

<div align="left"><figure><img src="../../.gitbook/assets/Picture2.png" alt="" width="496"><figcaption></figcaption></figure></div>

3\.     Click Add to create a new Index.

<div align="left"><figure><img src="../../.gitbook/assets/2020_01_21_15_24_08_edited_.png" alt=""><figcaption></figcaption></figure></div>

4\. Type in the correct formula for the Sensor and click OK.\
&#x20;     _Note: You can only use the formula that is valid for your sensor type._     &#x20;

&#x20;     **NDVI** = (nir-red)/(nir+red)\
&#x20;     **NDRE** = (nir-red\_edge)/(nir+red\_edge)

<div align="left"><figure><img src="../../.gitbook/assets/2020_01_21_15_25_28.png" alt=""><figcaption></figcaption></figure></div>

5\.  Give the index a meaningful name. Keeping in mind if this is an NDVI or NDRE sensor.  For example, Single Sensor NDVI.&#x20;

<div align="left"><figure><img src="../../.gitbook/assets/2020_01_21_15_24_08.png" alt=""><figcaption></figcaption></figure></div>

6\. Select the Index and click Generate.

<div align="left"><figure><img src="../../.gitbook/assets/2020_01_21_15_27_29.png" alt=""><figcaption></figcaption></figure></div>

**Downloads:**

{% tabs %}
{% tab title="Adding A Template to Pix4D" %}
{% file src="../../.gitbook/assets/Adding_a_Template_to_Pix4D.pdf" %}
{% endtab %}

{% tab title="Sentera Single Precision NDRE Template" %}
{% file src="../../.gitbook/assets/sentera_single_precision_NDRE_2020_01_20.tmpl" %}
{% endtab %}

{% tab title="Sentera Single Precision NDVI Template" %}
{% file src="../../.gitbook/assets/sentera_single_precision_NDVI_2020_01_20.tmpl" %}
{% endtab %}
{% endtabs %}
