# dsa2019addis

A DSA meeting webpage.

This repository contains the the details of a DSA meeting. 

## Creating a New Meeting. 

1. Create the new repo in github by going to <https://github.com/organizations/dalimeeting/repositories/new>, use the name coding `dsaXXXXcity` where `XXXX` is the year of the archived conference and city is an abbreviation for the city. 

2. In the conference description field, place the dates and location of the workshop, e.g. "21st-25th October, Accra, Ghana"

3. Do *not* create an initial README for the conference. 

4. Create the Repo.

5. Go to a suitable directory on your machine and type:

## Select a Suitable Previous Meeting to Copy From

Here we're basing the new repo on dsaconfstub

```
git clone --bare https://github.com/datsciafrica/dsaconfstub.git
mv dsaconfstub dsaXXXXcity.git
cd dsaXXXXcity.git
git branch -m gh-pages
git push --mirror https://github.com/datsciafrica/dsaXXXXcity.git
```
6. Now the repo is on line and you can clone it in the normal way to start working on it.

```
git clone https://github.com/datsciafrica/dsaXXXXcity.git
cd dsaXXXXcity
````

7. If everything is OK you can delete the bare mirror in the subdirectory ```dsaXXXXcity.git```.

8. Edit the `_config.yml` file in the new repo to set `baseurl` to `dsaXXXXcity` and set `permalink` to  `"/:title.html"`.

9. Commit the changes and push the repo.

10. Check that the archived page appears online at http://datascienceafrica.org/dsaXXXXcity.git

11. Add the team `dsaXXXXcity` to the admin rights for the repo `dsaXXXXcity`

12. Create a new admin team for this year's page, `dsaXXXXcity`, which contains program and general chairs for editing the page.

## More information

* See
  a list of repositories of past web sites [here](https://github.com/datsciafrica/).

* This link gives [Github help about project
pages](https://help.github.com/articles/user-organization-and-project-pages/)
(at the bottom), if we put the Jekyll files in **gh-pages** branch, the repository
will be served under http://datsciafrica.github.io/dsaXXXcity. Note that the *main*
repository uses master branch, not gh-pages.




