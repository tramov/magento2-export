# magento2-export

Connection between eboekhouden and magento2 

E-Boekhouden released a partial port of their Magento 1 module for Magento 2 (eboekhouden/magento2-export) back in 2016. 
The code is a basic port of the Magento 1 module and thankfully the E-Boekhouden API is very simple. 

This fork contains the required updates to make this code work with Magento 2.3.4

# Installation

Copy the code in the /src directory to a new directory /app/code/Eboekhouden/Export

Run 

* bin/magento module:enable Eboekhouden_Export
* bin/magento setup:upgrade

The configuration menu can be found under Stores > Configuration > Sales > E-Boekhouden. In addition you can link the proper taxes
to each of Magento's tax classes. 

# Warnings 

Migrated invoices and creditnotes do not contain enough information (shipping taxes) to properly export them to E-Boekhouden. 
Only export Magento 2 created invoices & credit notes. 






