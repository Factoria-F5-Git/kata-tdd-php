# phpunit setup

This is a simple bootstrap project for PHP with phpunit

For PHP 7.2 or above just run:

```
./composer install

```

To run the tests just run:

```
phpunit --bootstrap vendor/autoload.php tests --filter testNotFailing
```

You need PHP 7.2 or above.

If you have legacy version of php please change composer.json file
and include the version that is compatible with you version of PHP

If you change the phpunit version do not forget to run:

```
./composer update --with-dependencies

```

# run from docker

```
'./test.sh'
```

## Vehicle Rent Calculator kata

En la clase VehicleRentCalculator crear una funcion que:

- Calcule el precio de alquilar un coche, con una tarifa de 10 EUR por hora
- Calcule el precio de alquilar una furgoneta, con una tarifa de 15 EUR por hora
- Calcule el precio de alquilar un camion, con una tarifa de 30 EUR por hora
- Si el alquiler es de 24 horas o mas, la tarifa pasara a ser diaria, con un precio de 60 por dia en coches, 90 en furgonetas y 180 en camiones. Una fraccion de dia se paga como un dia entero
- Por alquilar un coche 3 dias o mas, se obtiene un dia de regalo
