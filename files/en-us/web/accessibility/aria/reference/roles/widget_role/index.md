---
title: "ARIA: widget role"
short-title: widget
slug: Web/Accessibility/ARIA/Reference/Roles/widget_role
page-type: aria-role
spec-urls: https://w3c.github.io/aria/#widget
sidebar: accessibilitysidebar
---

The **`widget`** role, an [abstract role](/en-US/docs/Web/Accessibility/ARIA/Reference/Roles#6._abstract_roles), is an interactive component of a graphical user interface (GUI).

> [!WARNING]
> The `widget` role is an abstract role used for the ontology. It is included here for completeness of documentation. It should not be used by web authors.

## Description

The abstract `widget` role is a superclass role for some interactive GUI elements and grouping roles. `role="widget"` should not be confused with widgets roles, such as `option`, `menuitem`, and `searchbox`.

The `widget` role is a superclass role several abstract interactive GUI roles, including [`command`](/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/command_role), [`composite`](/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/composite_role), [`input`](/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/input_role), [`range`](/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/range_role), and [`separator`](/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/separator_role) (if focusable), which should not be used by web authors.

The abstract `widget` role is also a superclass role for some grouping roles which can be used by web authors, including [`gridcell`](/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/gridcell_role), [`row`](/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/row_role), [`separator`](/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/separator_role) (when not focusable), and [`tab`](/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/tab_role), which can and should be used when appropriate. When the user navigates to one of these non-abstract roles of widget, keyboard events can switch to an application browsing mode, and pass keyboard events through to the browser.

## Specifications

{{Specifications}}

## See also

- [ARIA: `roletype` role](/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/roletype_role)

- [ARIA: `command` role](/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/command_role)
- [ARIA: `composite` role](/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/composite_role)
- [ARIA: `gridcell` role](/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/gridcell_role)
- [ARIA: `input` role](/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/input_role)
- [ARIA: `range` role](/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/range_role)
- [ARIA: `row` role](/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/row_role)
- [ARIA: `separator` role](/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/separator_role)
- [ARIA: `tab` role](/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/tab_role)
