# Go API Example

## To run integration test

```console
$ docker-compose -f docker-composer.test.yml up --build --abort-on-container-exit --exit-code-from it_tests
```

> `--build` ให้มัน build ตัวที่เป็น integration test
>
> `--abort-on-container-exit` ให้หยุดทำงานกรณีที่มี container ที่มันพัง
>
> `it_tests` จะ link กับไฟล์ `dockerfile: ./Dockerfile.test`

## To tear down integration test

```sh
$ docker-compose -f docker-composer.test.yml down
```