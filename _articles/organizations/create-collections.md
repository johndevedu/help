---
layout: article
title: Create a Collection
categories: [organizations]
featured: true
popular: false
tags: [collections, how to]
order: 05
redirect_from:
  - /article/how-to-manage-collections/
---

This article will guide you through the process of creating a Collection. For more information about Collections, see [About Collections](https://bitwarden.com/help/article/about-collections/).

## Create a Collection

Complete the following steps to create a collection:

1. Login to your [Web Vault](https://vault.bitwarden.com){:target="\_blank"} and open your Organization.
2. In your Organization, open the **Manage** tab and select **Collections** from the left menu.
3. On the **Collections** screen, select the **New Collection** button.

   {% image organizations/collection-list-overlay.png Select New Collection %}
4. On the **Add Collection** screen:
   - Enter a **Name** for your Collection.
   - Enter an **External Id** for your Collection. External ids are used to link resources to external systems, like user directories.
   - (*Teams and Enterprise Organizations*) Set the **Group Access** configuration for your Collection, including which Groups should be allowed to access this Collection. For more information, see [About Groups](https://bitwarden.com/help/article/about-groups/).
5. Select **Save** to finish creating your Collection.

## Create Nested Collections

Collections can be "nested" in order to logically organize them within your Vault. There's no limit to the depth with which you can nest Collections, but creating too many levels may interfere with your Vault's interface.

{% callout info %}
Nested Collections are designed for in-Vault display purposes only. Nested Collections will not not inherit access or permissions from their "parent" Collection.
{% endcallout %}

{% image organizations/collection-nested.png Nested Collection %}

To create a nested Collection, give your new Collection a **Name** that includes the "parent" Collection followed by a forward slash (`/`) delimiter, for example `Collection 1/Collection 1a`.

If there is no Collection with the corresponding "parent" name or if you don't have access to the "parent", the Collection won't nest and instead it's title will be displayed in-full.

{% image organizations/collection-nested-create.png Create a nested Collection %}

## Delete a Collection

Complete the following steps to delete a collection:

1. Login to your [Web Vault](https://vault.bitwarden.com){:target="\_blank"} and open your Organization.
2. In your Organization, open the **Manage** tab and select **Collections** from the left menu.
3. On the **Collections** screen, hover over the Collection you want to delete and select the gear dropdown.
4. From the gear dropdown, select **Delete**:

   {% image /organizations/collection-delete.png Delete a Collection %}

Deleting a Collection **will not** delete the Vault items in that Collection. When a Collection is deleted, Vault items will be moved to the {% icon fa-cube %} **Unassigned** filter in the Organization Vault view.




### Next Steps

Once you've created a Collection, we recommend that you:
- [Share Items to a Collection](https://bitwarden.com/help/article/share-to-a-collection/)
- [Import Items to an Organization](https://bitwarden.com/help/article/import-to-org/)
