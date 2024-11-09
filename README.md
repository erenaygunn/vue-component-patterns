# Vue 3 Component Patterns

This project showcases various Vue 3 component patterns. Below is a brief explanation of each pattern included in the project:

## Container/Presentational

- **Container Component**: Manages state and logic, passing data and actions to presentational components.
- **Presentational Component**: Focuses on how things look, receiving data and actions via props.
- **Example**: `Container.vue` and `Presentational.vue`

## Dynamic Components

- **Dynamic Components**: Allows switching between different components dynamically using the `<component>` element.
- **Example**: `Dynamic.vue`

## Mixins

- **Mixins**: Reusable pieces of functionality that can be included in multiple components.
- **Example**: `Mixin.vue` and `myMixin.js`

## Provide-Inject

- **Provide-Inject**: Allows parent components to provide data to their descendants, bypassing intermediate components.
- **Example**: `Parent.vue` and `Child.vue`

## Provider-Consumer

- **Provider-Consumer**: Similar to provide-inject but often used with slots to pass data to nested components.
- **Example**: `Provider.vue` and `Consumer.vue`

## Adapter

- **Adapter**: Wraps a third-party library or API to make it compatible with your application.
- **Example**: `Adapter.vue`

## FormBuilder

- **FormBuilder**: A pattern for building forms dynamically, often using slots to customize form fields.
- **Example**: `FormBuilder.vue`

## Functional

- **Functional Components**: Stateless components that are purely functional and do not have their own reactive data.
- **Example**: `Functional.vue`

## Renderless

- **Renderless Components**: Components that do not render any HTML themselves but provide behavior or data to other components via scoped slots.
- **Example**: `Renderless.vue`

## SFC (Single File Component)

- **Single File Component**: The standard way of writing Vue components, combining template, script, and style in a single file.
- **Example**: `SFC.vue`

## Slots

- **Slots**: A way to pass content from a parent component to a child component, allowing for flexible and reusable components.
- **Example**: `Slots.vue`

## Teleport

- **Teleport**: Allows you to render a component's template in a different part of the DOM tree.
- **Example**: `Teleport.vue`

## Template Literal

- **Template Literal**: Using JavaScript template literals to dynamically generate HTML content.
- **Example**: `TemplateLiteral.vue`
