# D-Code Beauty 

Topic modeling on beauty products to determine ingredients origin groups


## General Info

This project was made to present as a Final Project for LeWagon's DataScience Bootcamp (Batch 840).

Its purpose remains on bringing together all the components learnt during the bootcamp on a real open-ended problem.

## Problem to solve

The demand of natural and organic base products has risen in the last years exponencially, consumers have used their purchasing power to prioritize health, wellness, and the environment. Nielsen found that 73 per cent of consumers would likely make purchases based on whether there would be a reduced impact on the environment, and 41 per cent are willing to pay more to do so by buying all-natural and organic goods. 
But buying organic base beauty products is really difficult beacuse ingredients are not regulated by law and its not mandatory to describe products in the product labels. 
That's when Dcode-Beauty come´s handy. We can scan the list of the ingredients from the label or type the name of the product and the app tell's us the origin of the product.

## Demo

You can go to the web app: https://dcodebeauty.herokuapp.com/


## Project

### Data Source

--> Web Scraping - https://incidecoder.com/
We scrape the descriptions of the products base on their INCI name, a unique name of each ingredient.

--> API: - https://github.com/LauraRobertson/skincareAPI

We got every INCI name of each ingredient available in the products and a library with the comercial name of a product and the ingredients it contains.

## Site

In the site we can find many options to check our product.

![web principal](https://user-images.githubusercontent.com/98696646/192239842-50fe646f-deac-4010-a245-a4fc48d0364c.png)


# Startup the project

The initial setup.

Create virtualenv and install the project:
```bash
sudo apt-get install virtualenv python-pip python-dev
deactivate; virtualenv ~/venv ; source ~/venv/bin/activate ;\
    pip install pip -U; pip install -r requirements.txt
```

Unittest test:
```bash
make clean install test
```

Check for dcode-beauty in gitlab.com/{group}.
If your project is not set please add it:

- Create a new project on `gitlab.com/{group}/dcode-beauty`
- Then populate it:

```bash
##   e.g. if group is "{group}" and project_name is "dcode-beauty"
git remote add origin git@github.com:{group}/dcode-beauty.git
git push -u origin master
git push -u origin --tags
```

Functionnal test with a script:

```bash
cd
mkdir tmp
cd tmp
dcode-beauty-run
```

# Install

Go to `https://github.com/{group}/dcode-beauty` to see the project, manage issues,
setup you ssh public key, ...

Create a python3 virtualenv and activate it:

```bash
sudo apt-get install virtualenv python-pip python-dev
deactivate; virtualenv -ppython3 ~/venv ; source ~/venv/bin/activate
```

Clone the project and install it:

```bash
git clone git@github.com:{group}/dcode-beauty.git
cd dcode-beauty
pip install -r requirements.txt
make clean install test                # install and test
```
Functionnal test with a script:

```bash
cd
mkdir tmp
cd tmp
dcode-beauty-run
```
