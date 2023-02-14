https://github.com/angular-eslint/angular-eslint/issues/1311

This reproduces a new Angular 15 project configured with @angular-eslint
and using the @typescript-eslint/member-ordering rule.

Trying to `ng lint` results in the following error:

```
An unhandled exception occurred: .eslintrc.json#overrides[0]:
        Configuration for rule "@typescript-eslint/member-ordering" is invalid:
        Value ["signature","public-static-field","protected-static-field","private-static-field","public-decorated-field","protected-decorated-field","private-decorated-field","public-instance-field","protected-instance-field","private-instance-field","public-abstract-field","protected-abstract-field","private-abstract-field","public-constructor","protected-constructor","private-constructor","public-static-method","protected-static-method","private-static-method","public-decorated-method","protected-decorated-method","private-decorated-method","public-instance-method","protected-instance-method","private-instance-method","public-abstract-method","protected-abstract-method","private-abstract-method"] should be string.
        Value ["signature","public-static-field","protected-static-field","private-static-field","public-decorated-field","protected-decorated-field","private-decorated-field","public-instance-field","protected-instance-field","private-instance-field","public-abstract-field","protected-abstract-field","private-abstract-field","public-constructor","protected-constructor","private-constructor","public-static-method","protected-static-method","private-static-method","public-decorated-method","protected-decorated-method","private-decorated-method","public-instance-method","protected-instance-method","private-instance-method","public-abstract-method","protected-abstract-method","private-abstract-method"] should be equal to one of the allowed values.
        Value "private-abstract-field" should be equal to one of the allowed values.
        Value "private-abstract-field" should be array.
        Value "private-abstract-field" should match exactly one schema in oneOf.
        Value ["signature","public-static-field","protected-static-field","private-static-field","public-decorated-field","protected-decorated-field","private-decorated-field","public-instance-field","protected-instance-field","private-instance-field","public-abstract-field","protected-abstract-field","private-abstract-field","public-constructor","protected-constructor","private-constructor","public-static-method","protected-static-method","private-static-method","public-decorated-method","protected-decorated-method","private-decorated-method","public-instance-method","protected-instance-method","private-instance-method","public-abstract-method","protected-abstract-method","private-abstract-method"] should be object.
        Value ["signature","public-static-field","protected-static-field","private-static-field","public-decorated-field","protected-decorated-field","private-decorated-field","public-instance-field","protected-instance-field","private-instance-field","public-abstract-field","protected-abstract-field","private-abstract-field","public-constructor","protected-constructor","private-constructor","public-static-method","protected-static-method","private-static-method","public-decorated-method","protected-decorated-method","private-decorated-method","public-instance-method","protected-instance-method","private-instance-method","public-abstract-method","protected-abstract-method","private-abstract-method"] should match exactly one schema in oneOf.
```
