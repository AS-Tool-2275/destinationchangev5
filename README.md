# Destination Change - Streamlit Package

## Main files
- destination_change_streamlit_app.py - Streamlit entry point
- destination_change_unified_flow.py - backend logic
- requirements.txt - dependencies

## New Firm Target behavior
Priority Mode = FIRM now supports a warehouse-level Firm Target.
- Target < Original Firm: reduce Firm from the warehouse using SS% highest first, then redistribute PCS to eligible same-item warehouses.
- Target = Original Firm: no Firm redistribution for that warehouse.
- Target > Original Firm: add Firm to the warehouse using lowest SS% recipient logic, funded by eligible donor warehouses with higher SS%.
- Existing Hard Lock / HB / Priority Rank / Sequential Firm Waterfall behavior remains in place.
