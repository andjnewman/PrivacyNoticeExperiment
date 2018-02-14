---
layout: default
---

{% for metarec in site.data.goatlicences %}
{% if metarec.URI == "12345" %}

# Privacy Notice

We (**_{{ metarec.Controller }}_**) are committed to the responsible handling and security of personal data.  Your privacy is important to us and protected in law through the General Data Protection Regulation (GDPR) and other legislation, including the Data Protection Act 2018.  We must provide you with information setting out how we process your personal data.

### What is personal data?
Personal data, is data which identifies an individual directly or indirectly, in particular by reference to an identifier such as their name or a reference number.

Some personal data is more sensitive in nature and requires more careful handling.  GDPR defines “special categories of personal data” which means data relating to a living person’s racial or ethnic origin, political opinions, religious or philosophical beliefs, or trade union membership, genetic data, biometric data, data concerning health or data concerning someone’s sex life or sexual orientation.

## What data is being collected?

### Name of data:###

**_{{ metarec.Title }}_**

### Decription of data:

**_{{ metarec.Abstract }}_**

## Who is collecting it?

**_{{ metarec.Controller }}_** is the data controller for this personal data. Your personal data will be protected in line with the GDPR and any other relevant legislation.  **_{{ metarec.Controller }}_** is responsible for overseeing data protection strategy and implementation to ensure compliance with legal requirements.  **_{{ metarec.Controller }}_** will provide the Information Commissioner’s Office (ICO) with details about how it processes personal data.

Contact the **_{{ metarec.Controller }}_**'s Data Protection Officer if you have any questions, or concerns about the handling of your personal information.


{% if metarec.Controller == "Goat Regulating Agency" %}
   **_{{ metarec.Controller }}_**
   
   **_Goat HQ, Jones Square, London_**
   
   **_Phone: 04056 156156_**
   
   **_Email: gdpr@goats.gov.uk_**
    
{% else %}

   **_Add address to lookup _**

{% endif %}

## How we use your data?
We process your personal data in a number of ways to deliver Public Services.

{% if metarec.LegalBasisProcessing == "Public interest" %}
   
   **_We are processing this data to deliver a service that is in the public interest_**
    
{% else %}

   **_Add other legal basis to lookup _**

{% endif %}

### Purpose of processing this data

**_{{ metarec.PurposeOfProcessing }}_**

### Data Capture and Storage

**_{{ metarec.Source }}_**

**_{{ metarec.DataFormat }}_**

### Data Security Rating

**_{{ metarec.DataSecurity }}_**

### Data retention

**_{{ metarec.RetentionSchedule }}_**

## Who will it be shared with?

Data Processors are responsible for processing personal data on behalf of a controller. Data processors have specific legal obligations; for example, they are required to maintain records of personal data and processing activities. Each processor has a legal liability if they are responsible for a breach.

The following organisations process this personal data:

{% if metarec.Processor == "" %}

Only the data controller processes this data.

{% else %}

**_{{ metarec.Processor }}_**

### How do these processors access the data?

**_{{ metarec.DataSharing }}_**

{% endif %}

### is the data processed outside the UK?

{% if metarec.OverseasProcessing == "Yes" %}

The data **_is_** processed outside the UK.   
    
{% else %}

The data **_is not_** processed outside the UK.   

{% endif %}



<!--

How is it collected?
Why is it being collected?
How will it be used?
What will be the effect of this on the individuals concerned?
Is the intended use likely to cause individuals to object or complain?
And as per the GDPR it must include the following points for clarification:
Purposes and legal basis of processing
Recipients of data
Retention period or criteria (summarise and put in the link to the processes – Stephen)
Right to request rectification
The data subject shall have the right to obtain from the controller without undue delay the rectification of inaccurate personal data concerning him or her. Taking into account the purposes of the processing, the data subject shall have the right to have incomplete
personal data completed, including by means of providing a supplementary statement
Right to request we no longer process your personal data
Source of Data (Supply from a third party)

Consequences of failure to supply data

-->

## How do I make a complaint about how my personal data has been handled?
If you think your data has been misused or that it hasn’t kept it secure, you should contact the Data Protection Officer identifeid at section 2.

### Right to complain to the ICO

If you’re unhappy with their response or if you need any advice you should contact the Information Commissioner’s Office (ICO) who are the supervisory authority.

Information Commissioner's Office
Wycliffe House
Water Lane
Wilmslow
Cheshire
SK9 5AF
0303 123 1113
casework@ico.org.uk

Any complaint to the Information Commissioner is without prejudice to your right to seek redress through the courts. 

## Changes to this policy

When we make changes, such as where legislation changes, we will update this notice and do our best to let you know.  We can only do this, if you let us have your contact details, your preferred forms of communication and you inform us of any changes.

{% endif %}
{% endfor %}
