---
date: '2025-12-05'
---
# Inventory Pending Deletion in Ansible Automation Platform


### Load Django Shell
```
sudo awx-manage shell_plus
```

### Display inventory
```
from awx.main.models import Inventory
```
```
Inventory.objects.all()
```
### Delete inventory based on id
```
Inventory.objects.filter(id=168).delete()
```

### Display inventory (pending delete)
```
Inventory.objects.filter(pending_deletion=True)
```
