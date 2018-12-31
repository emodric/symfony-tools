# ezsystems/symfony-tools
Collection of polyfill (backport) and incubator features for Symfony.

Backports Symfony features so they can be used in earlier versions of Symfony, and 
aims to serve as incubator for ideas to improve Symfony in the future.

This bundle is first and foremost aiming to cover needs of [eZ Platform](https://ezplatform.com),
but is placed in own bundle under MIT as we think others can benefit and help collaborate, and
to simplify forward and backport ports to and from Symfony itself.

### Requriments

- Symfony 3.4 _(4.3+ planned spring 2019, 2.8 support might happen if we need it)_
- PHP 5.6+ v1 for Symfony 3/2, PHP 7.1+ in v2 for Symfony 4

#### Semantic Versioning exception

Bundle follows [SemVer](https://semver.org/) with one exception:
- Incubator features are allowed to break BC also in Minor versions (x.Y.z), __when__ needed in order to align with changes to the feature when it gets contributed to Symfony.


!! Tip:  As such if you rely on incubator features, make sure to require specific minor versions in composer, like `~1.1.0` or `~1.1.2 || ~1.2.0`

### Features

*Only listing of features (further info in `doc/<feature>.md`):*

**Polyfill (Backports) features:**
- 

**Incubator features**
- 


### Contributing

Make sure as much as possible the feature is forward compatible for users, so when they upgrade to Symfony version where it's included, they not need to adapt their code/config. _(see `Semantic Versioning exception` for how this works for incubators)_

**Polyfill (Backports)**
When contributing Symfony backports to this bundle, be aware you commit to help maintain that feature in case there are bug fixes or improvements to that feature in Symfony itself.

**Incubator**
Incubator features should only be proposed here if you intend to contribute this to Symfony itself, and there is at least some certainty it will be accepted. And you also commit to adapt the feature here, if changes are requested once proposed to Symfony.

As such it's only applicable for smaller features _(e.g. new cache adapter)_, not a complete new component for instance. 

### License

[The MIT License](LICENSE).
