---
title: \leantime\core\controller
footer: false
---

# controller





* Full name: `\leantime\core\controller`



## Methods

### __construct

constructor - initialize private variables

```php
public controller::__construct( $method,  $params): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `method` | **** | the method to be initialized |
| `params` | **** | parameters or body of the request |


**Return Value:**





---
### executeActions

Allows hooking into all controllers with events

```php
private controller::executeActions(string $method, array|object $params): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `method` | **string** |  |
| `params` | **array|object** |  |


**Return Value:**





---
### init

Extended Controller version of __construct()

```php
protected controller::init(): void
```









**Return Value:**





---
### run

Default function for all request types unless otherwise specified

```php
protected controller::run(): void
```









**Return Value:**





---


## Inherited methods

### dispatch_event

dispatches an event with context

```php
public static eventhelpers::dispatch_event(string $hook, mixed $available_params = [], string|int $function = null): void
```



* This method is **static**.




**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `hook` | **string** |  |
| `available_params` | **mixed** |  |
| `function` | **string|int** |  |


**Return Value:**





---
### dispatch_filter

dispatches a filter with context

```php
public static eventhelpers::dispatch_filter(string $hook, mixed $payload, mixed $available_params = [], string|int $function = null): mixed
```



* This method is **static**.




**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `hook` | **string** |  |
| `payload` | **mixed** |  |
| `available_params` | **mixed** |  |
| `function` | **string|int** |  |


**Return Value:**





---
### get_event_context

Gets the context of the event

```php
private static eventhelpers::get_event_context(mixed $function): string
```



* This method is **static**.




**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `function` | **mixed** |  |


**Return Value:**





---
### set_class_context

Gets the class context based on path, this uses the same method as the autoloader
Helps create unique strings for events/filters

```php
private static eventhelpers::set_class_context(): string
```



* This method is **static**.





**Return Value:**





---
### get_function_context

Gets the caller function name

```php
private static eventhelpers::get_function_context(mixed $functionInt = null): string
```

This way we don't have to use much memory by using debug_backtrace

* This method is **static**.




**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `functionInt` | **mixed** |  |


**Return Value:**





---


---
> Automatically generated from source code comments on 2023-02-28 using [phpDocumentor](http://www.phpdoc.org/)
