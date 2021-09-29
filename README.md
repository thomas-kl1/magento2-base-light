# Setup:

First of all, please install a theme, you can use the Magento luma one:
(By default luma is installed, remove it first)

        "magento/theme-frontend-luma": "*"

Then install an elasticsearch package if you want to:
(By default v7 is installed, remove it first)

        "magento/module-elasticsearch-6": "*",
        "magento/module-elasticsearch-7": "*",

You can now install the Magento software:

magento setup:install --base-url=http://opengent-cms.local.com/ \
--db-host=localhost --db-name=opengento_base --db-user=root \
--admin-firstname=Magento --admin-lastname=User --admin-email=admin@example.com \
--admin-user=admin --admin-password=admin123 --language=en_US \
--currency=USD --timezone=America/Chicago --cleanup-database \
--sales-order-increment-prefix="ORD$" --session-save=db --use-rewrites=1 \
--search-engine=elasticsearch7 --elasticsearch-host=localhost \
--elasticsearch-port=9200

# Extra modules


Install advanced cookie management:
        "magento/module-cookie": "*",
