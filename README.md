# Sekoliko build status : [![CircleCI](https://circleci.com/gh/julkwel/sekoliko/tree/develop.svg?style=svg)](https://circleci.com/gh/julkwel/sekoliko/tree/develop)
[![All Contributors](https://img.shields.io/badge/all_contributors-12-orange.svg?style=flat-square)](#contributors)

School Management Web Application OPENSOURCE
![sekoliko](https://raw.githubusercontent.com/julkwel/sekoliko/develop/public/images/demo.png)

## Requirements
```
- composer
- node && yarn
- php > 7.2
- symfony cli (link to download: https://symfony.com/download)
- motivation
- basics of symfony & php
- basics of Javascript
```
## Usage
Step 1. Fork this project

Step 2. 

`- git clone https://github.com/[your_username]/sekoliko.git`

Step 3. Create new branch [optional] (if you want to contribute)

`- git checkout -b feature/my-branch`

Step 4. Install composer dependencies

`- composer install` 

Step 5. Install node dependencies

`- yarn install`

Step 6. Create new database then, create new file `.env.local`, add `.env` content to this and configure DATABASE_URL in `.env.local` to follow your own database configuration like :

`- DATABASE_URL="mysql://db_user:db_password@127.0.0.1:3306/db_name?serverVersion=5.7"`

Step 7. Update database schema

`- php bin/console doctrine:schema:update --force`

Step 6. Run server

`- symfony serve`

Step 7. Run webpack server for assets

`- yarn encore dev --watch`

Create your first user by running :

`php bin/console sekoliko:create:super-admin`

For new school and admin run :

`php bin/console sekoliko:create:admin`

## STANDARD

Code must follow [symfony coding standard style](https://symfony.com/doc/current/contributing/code/standards.html),Install this coding standard in your root directory of sekoliko.

```
git clone git://github.com/djoos/Symfony2-coding-standard.git && composer install -d ./Symfony2-coding-standard
./Symfony2-coding-standard/vendor/bin/phpcs --config-set installed_paths ../../../../Symfony2-coding-standard
```

Then run this command ALWAYS and fix all errors before your push.

```
./Symfony2-coding-standard/vendor/bin/phpcs --standard=Symfony --ignore=*/vendor/*,/src/Kernel.php,*/Migrations/* ./src/
```

## Design 
Make cool and user friendly design, we have a template named `admirator` inside assets directory for theme.

## Git
Commit convention :
 - All commit MUST be tagged with one of the following tags : [bug] / [fix] / [feature] / [design] / [packages] / [wip]
 - DON'T create merge request for unstable developpment.
 - All code must be passed with TU/TF.
 
## Goal 
- SaaS (Software as a Service ) App for School/University in Madagascar
- Online course
- Online report
- Fee management
- Student/Teachers/Administration management ( attendance, year sumary )
- Classroom management for thos school who doesn't have fixed room.

## NON Goal
- Online university.

____
**Make cool things :wink:**
____
## Contributors ✨

Thanks goes to these wonderful people :

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore -->
<table>
  <tr>
    <td align="center"><a href="https://heuristic-raman-24225d.netlify.com"><img src="https://avatars1.githubusercontent.com/u/40351002?v=4" width="100px;" alt="SylvanoTombo"/><br /><sub><b>SylvanoTombo</b></sub></a><br /><a href="https://github.com/julkwel/sekoliko/commits?author=SylvanoTombo" title="Code">💻</a></td>
    <td align="center"><a href="https://github.com/RinaVatosoa"><img src="https://avatars2.githubusercontent.com/u/45585022?v=4" width="100px;" alt="RinaVatosoa"/><br /><sub><b>RinaVatosoa</b></sub></a><br /><a href="#design-RinaVatosoa" title="Design">🎨</a></td>
    <td align="center"><a href="https://www.devinart.net/"><img src="https://avatars0.githubusercontent.com/u/35923219?v=4" width="100px;" alt="nyantso"/><br /><sub><b>nyantso</b></sub></a><br /><a href="https://github.com/julkwel/sekoliko/commits?author=Nantso" title="Code">💻</a></td>
    <td align="center"><a href="https://github.com/Fy-Rakotondrabe"><img src="https://avatars2.githubusercontent.com/u/45007981?v=4" width="100px;" alt="Fy Kely"/><br /><sub><b>Fy Kely</b></sub></a><br /><a href="https://github.com/julkwel/sekoliko/commits?author=Fy-Rakotondrabe" title="Code">💻</a> <a href="#design-Fy-Rakotondrabe" title="Design">🎨</a></td>
    <td align="center"><a href="https://github.com/chrys-elrak"><img src="https://avatars0.githubusercontent.com/u/40733956?v=4" width="100px;" alt="Chrys Rakotonimanana"/><br /><sub><b>Chrys Rakotonimanana</b></sub></a><br /><a href="https://github.com/julkwel/sekoliko/commits?author=chrys-elrak" title="Code">💻</a></td>
    <td align="center"><a href="https://cvjulien.netlify.com/"><img src="https://avatars0.githubusercontent.com/u/30557565?v=4" width="100px;" alt="Jul"/><br /><sub><b>Jul</b></sub></a><br /><a href="#projectManagement-julkwel" title="Project Management">📆</a> <a href="#review-julkwel" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/julkwel/sekoliko/commits?author=julkwel" title="Tests">⚠️</a> <a href="https://github.com/julkwel/sekoliko/commits?author=julkwel" title="Code">💻</a></td>
    <td align="center"><a href="https://www.facebook.com/hantsaniala"><img src="https://avatars1.githubusercontent.com/u/8157490?v=4" width="100px;" alt="Hantsaniala Eléo"/><br /><sub><b>Hantsaniala Eléo</b></sub></a><br /><a href="#design-hantsaniala" title="Design">🎨</a></td>
  </tr>
  <tr>
    <td align="center"><a href="http://tolotrasmile.github.io"><img src="https://avatars3.githubusercontent.com/u/8298581?v=4" width="100px;" alt="Tolotra Raharison"/><br /><sub><b>Tolotra Raharison</b></sub></a><br /><a href="https://github.com/julkwel/sekoliko/commits?author=tolotrasmile" title="Code">💻</a></td>
    <td align="center"><a href="https://github.com/vonyms"><img src="https://avatars3.githubusercontent.com/u/33556409?v=4" width="100px;" alt="Vony Randria"/><br /><sub><b>Vony Randria</b></sub></a><br /><a href="https://github.com/julkwel/sekoliko/commits?author=vonyms" title="Code">💻</a></td>
    <td align="center"><a href="https://github.com/max5055"><img src="https://avatars1.githubusercontent.com/u/39415739?v=4" width="100px;" alt="rhianmax"/><br /><sub><b>rhianmax</b></sub></a><br /><a href="https://github.com/julkwel/sekoliko/commits?author=max5055" title="Code">💻</a></td>
    <td align="center"><a href="https://github.com/HenintsoaHARINORO"><img src="https://avatars2.githubusercontent.com/u/48785203?v=4" width="100px;" alt="Henintsoa Harinoro"/><br /><sub><b>Henintsoa Harinoro</b></sub></a><br /><a href="#translation-HenintsoaHARINORO" title="Translation">🌍</a></td>
    <td align="center"><a href="https://mikaoelitiana.name"><img src="https://avatars0.githubusercontent.com/u/674667?v=4" width="100px;" alt="Mika Andrianarijaona"/><br /><sub><b>Mika Andrianarijaona</b></sub></a><br /><a href="https://github.com/julkwel/sekoliko/commits?author=mikaoelitiana" title="Code">💻</a> <a href="https://github.com/julkwel/sekoliko/commits?author=mikaoelitiana" title="Documentation">📖</a></td>
  </tr>
</table>

<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome !
