![assetEditor-update](https://github.com/JohnRSim/OCM-GO/assets/364208/763b7a31-67be-4e2e-a894-a9b410ef653a)

# Overview
__OCM Go__ is a new Desktop App; designed to enhance the editor experience of Oracle Content Management Assets via a local network drive. 
Enabling editors to quickly and more easily manage and drill into an OCM Repository and taxonomy category folders to access, edit and update assets faster.  

https://bitmapbytes.com/oracle-content-managements-new-desktop-app-coming-soon/



https://github.com/JohnRSim/OCM-GO/assets/364208/87f19e2e-1caf-4afc-8e68-75c954c44907



# Download
Coming soon.. 

- Windows
- Mac (WIP)

# Prerequisite
_OCM-GO runs as an internal local server_

To enable the app to access to your OCM instance and APIs - you will need to configure the OCM Security Policy.

1. Launch your OCM instance within a web browser
2. Go into Administration >> System >> Security
3. Add http://127.0.0.1:5173 to Front Channel CORS Origins & Allowed domains
4. Select Enable Radio on the Embedded Content
5. Select Save button

![image](https://github.com/JohnRSim/OCM-GO/assets/364208/53eeefd8-e340-44bc-aca0-343a50696cd5)

#### Note
If you do not do this on the instance or configure it incorrectly in OCM you will just see a white page when you add your OCM Instance into OCM-GO.

# Features Quick Overview & Guide
- [Installation](https://github.com/JohnRSim/OCM-GO/wiki/Installation)

### OCM-GO Desktop App
- [Create connections to login to multiple OCM instances](https://github.com/JohnRSim/OCM-GO/wiki/Add-OCM-Instance)
- Enable one or more Virtual drives 
- Search for assets
- Add a single asset to favourites or create a favourites bucket
- Save search query
- Configure OCM instance

### OCM-GO Virtual Drive
#### Folders (Taxonomy Categories)
-	Create, Rename, Delete, Move
#### Digital Assets
- Create, Rename, Update, Delete, Move
#### Assets
- Edit Meta Data (use OCM Go and Open-With feature in windows to edit meta data of assets within the OCM-GO App)


### Virtual Drive Structure
When you enable the virtual drive it is made up of 3 key folders.
- The root level which are a list of repositories on the OCM Instance.
- - Drilling into a repository will then list all taxonomies you have access to within the repository
- - - Drilling into a taxonomy will list all Categories you have access to

![image](https://github.com/JohnRSim/OCM-GO/assets/364208/b94c50e5-c875-48e7-9b6e-7778061acfc1)

#### Note
- Assets that are mapped to categories are displayed when opening a category folder.
- Assets that are not mapped to a category will not be available or listed within the virtual drive.

#### Limitations
- Folders are restricted to list only 5,000 assets

### Important
- You cannot rename a Repository or Taxonomy from the virtual drive. 
- If you try to delete a repository all assets and categories from the repository will be removed for the taxonomies you have access to.. _(the taxonomy and repository will remain.)_
- Assets that are referenced will not be deleted until the reference is manually removed.
- *.OCMA Files cannot be moved or deleted currently - you can only edit these using the open-with OCM-GO feature.
- Moving a digital asset from one folder to another will clear all other associated categories and will be replaced with the target category location


---

Shield: [![CC BY-NC-ND 4.0][cc-by-nc-nd-shield]][cc-by-nc-nd]

This work is licensed under a
[Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License][cc-by-nc-nd].

[![CC BY-NC-ND 4.0][cc-by-nc-nd-image]][cc-by-nc-nd]

[cc-by-nc-nd]: https://creativecommons.org/licenses/by-nc-nd/4.0/
[cc-by-nc-nd-image]: https://licensebuttons.net/l/by-nc-nd/4.0/88x31.png
[cc-by-nc-nd-shield]: https://img.shields.io/badge/License-CC%20BY--NC--ND%204.0-lightgrey.svg
