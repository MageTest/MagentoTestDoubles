# Magento Test Doubles

One of the big obstacles that developers face when attempting to write tests for
Magento is the untestability of the Magento core; no better example other than
the Magento god class, Mage.

The god class in magento is used for all sort of operations, from model factory
methods like Mage::getModel() to retrieval of configuration values from the database
using Mage::getConfig().

Unfortunately the use of this God class makes the code untestable for several
reasons:

- Tightly coupled code.
- Highly dependent of the database.

MagentoTestDoubles is a PHPSpec extension intended to provide a way to mock the Magento
god class using the [Patchwork](https://github.com/antecedent/patchwork) library.

Patchwork allows to redefine user-defined functions during runtime. For a quick proof
of concept example please look [here](https://github.com/amacgregor/magespec_patchwork_example)


## Installation 

## Prerequisites



