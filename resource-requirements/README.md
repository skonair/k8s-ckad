resources are CPU, memory and disk space

default: 0.5 cpu, 256Mi Mem if previously set via limit ranges

---
apiVersion: v1
kind: LimitRange
metadata:
  name: mem-limit-range
spec:
  limits:
  - default:
      memory: 512Mi
    defaultRequest:
      memory: 512Mi
    type: Container
---
apiVersion: v1
kind: LimitRange
metadata:
  name: cpu-limit-range
spec:
  limits:
  - default:
      cpu: 1
    defaultRequest:
      cpu: 0.5
    type: Container

1G (Gigabyte)  = 1,000,000,000 bytes
1M (Megabyte)  = 1,000,000 bytes
1K (Kilobyte)  = 1,000 bytes

1Gi (Gibibyte)  = 1,073,741,824 bytes
1Mi (Mebibyte)  = 1,048,576 bytes
1Ki (Kibibyte)  = 1,024 bytes

