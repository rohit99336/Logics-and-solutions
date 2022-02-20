## Various Faker Formatters

## useful links

1. [Updated Official Fekar Documetation](https://fakerphp.github.io/formatters/internet/)
2. [Core Official Documentation](https://faker.readthedocs.io/en/master/providers/faker.providers.date_time.html)
3. [Generating Fake Data in PHP With Faker](https://anchetawern.github.io/blog/2016/01/28/generating-fake-data-in-php-with-faker/)
4. [Generate Fake Data Using Laravel Faker](https://codeandtuts.com/generate-fake-data-using-laravel-faker/)
5. [PHP fekar parameters with argumets](https://zetcode.com/php/faker/) 

### Faker not only generate first name, last name but its also generate wide range of data shown as below. ( [refrence link](https://codeandtuts.com/generate-fake-data-using-laravel-faker/))

    // Base
    $faker->randomDigit             // 7
    $faker->randomDigitNotNull      // 5
    $faker->randomNumber($nbDigits = NULL, $strict = false) // 79907610
    $faker->randomFloat($nbMaxDecimals = NULL, $min = 0, $max = NULL) // 48.8932
    $faker->numberBetween($min = 1000, $max = 9000) // 8567
    $faker->randomLetter            // 'b'


    // returns randomly ordered subsequence of a provided array
    $faker->randomElements($array = array ('a','b','c'), $count = 1) // array('c')
    $faker->randomElement($array = array ('a','b','c')) // 'b'
    $faker->shuffle('hello, world') // 'rlo,h eoldlw'
    $faker->shuffle(array(1, 2, 3)) // array(2, 1, 3)
    $faker->numerify('Hello ###') // 'Hello 609'
    $faker->lexify('Hello ???') // 'Hello wgt'
    $faker->bothify('Hello ##??') // 'Hello 42jz'
    $faker->asciify('Hello ***') // 'Hello R6+'
    $faker->regexify('[A-Z0-9._%+-]+@[A-Z0-9.-]+\.[A-Z]{2,4}'); // sm0@y8k96a.ej

    // Person
    $faker->title($gender = null|'male'|'female')     // 'Ms.'
    $faker->titleMale                                 // 'Mr.'
    $faker->titleFemale                               // 'Ms.'
    $faker->suffix                                    // 'Jr.'
    $faker->name($gender = null|'male'|'female')      // 'Dr. Zane Stroman'
    $faker->firstName($gender = null|'male'|'female') // 'Maynard'
    $faker->firstNameMale                             // 'Maynard'
    $faker->firstNameFemale                           // 'Rachel'
    $faker->lastName                                  // 'Zulauf'

    // Address
    $faker->cityPrefix                          // 'Lake'
    $faker->secondaryAddress                    // 'Suite 961'
    $faker->state                               // 'NewMexico'
    $faker->stateAbbr                           // 'OH'
    $faker->citySuffix                          // 'borough'
    $faker->streetSuffix                        // 'Keys'
    $faker->buildingNumber                      // '484'
    $faker->city                                // 'West Judge'
    $faker->streetName                          // 'Keegan Trail'
    $faker->streetAddress                       // '439 Karley Loaf Suite 897'
    $faker->postcode                            // '17916'
    $faker->address                             // '8888 Cummings Vista Apt. 101, Susanbury, NY 95473'
    $faker->country                             // 'Falkland Islands (Malvinas)'
    $faker->latitude($min = -90, $max = 90)     // 77.147489
    $faker->longitude($min = -180, $max = 180)  // 86.211205

    // Phone Number
    $faker->phoneNumber             // '201-886-0269 x3767'
    $faker->tollFreePhoneNumber     // '(888) 937-7238'
    $faker->e164PhoneNumber     // '+27113456789'