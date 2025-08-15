kubectl apply -f daemonset.yml
kubectl apply -f cronjob.yml

todoapp-daemonset-jdfb5 
apiVersion: v1
kind: Pod
metadata:
  creationTimestamp: "2025-08-15T13:08:17Z"
  generateName: todoapp-daemonset-
  generation: 1
  labels:
    app: todoapp-daemonset
    controller-revision-hash: 8644898c47
    pod-template-generation: "2"
  name: todoapp-daemonset-jdfb5
  namespace: mateapp
  ownerReferences:
  - apiVersion: apps/v1
    blockOwnerDeletion: true
    controller: true
    kind: DaemonSet
    name: todoapp-daemonset
    uid: 65cf45da-1146-4baf-9473-f2f8f997dc2f
  resourceVersion: "21151"
  uid: 9209223e-9193-466e-8a07-d53940df8dc2
spec:
  affinity:
    nodeAffinity:
      requiredDuringSchedulingIgnoredDuringExecution:
        nodeSelectorTerms:
        - matchFields:
          - key: metadata.name
            operator: In
            values:
            - kind-worker2
  containers:
  - args:
    - |
      while true; do
        curl -f http://todoapp-svc-cip.mateapp.svc.cluster.local
        sleep 5
      done
    command:
    - /bin/sh
    - -c
    image: ikulyk404/busyboxplus:curl
    imagePullPolicy: IfNotPresent
    name: busybox
    resources:
      limits:
        cpu: 200m
        memory: 256Mi
      requests:
        cpu: 100m
        memory: 128Mi
    terminationMessagePath: /dev/termination-log
    terminationMessagePolicy: File
    volumeMounts:
    - mountPath: /var/run/secrets/kubernetes.io/serviceaccount
      name: kube-api-access-sjrvk
      readOnly: true
  dnsPolicy: ClusterFirst
  enableServiceLinks: true
  nodeName: kind-worker2
  preemptionPolicy: PreemptLowerPriority
  priority: 0
  restartPolicy: Always
  schedulerName: default-scheduler
  securityContext: {}
  serviceAccount: default
  serviceAccountName: default
  terminationGracePeriodSeconds: 30
  tolerations:
  - effect: NoExecute
    key: node.kubernetes.io/not-ready
    operator: Exists
  - effect: NoExecute
    key: node.kubernetes.io/unreachable
    operator: Exists
  - effect: NoSchedule
    key: node.kubernetes.io/disk-pressure
    operator: Exists
  - effect: NoSchedule
    key: node.kubernetes.io/memory-pressure
    operator: Exists
  - effect: NoSchedule
    key: node.kubernetes.io/pid-pressure
    operator: Exists
  - effect: NoSchedule
    key: node.kubernetes.io/unschedulable
    operator: Exists
  volumes:
  - name: kube-api-access-sjrvk
    projected:
      defaultMode: 420
      sources:
      - serviceAccountToken:
          expirationSeconds: 3607
          path: token
      - configMap:
          items:
          - key: ca.crt
            path: ca.crt
          name: kube-root-ca.crt
      - downwardAPI:
          items:
          - fieldRef:
              apiVersion: v1
              fieldPath: metadata.namespace
            path: namespace
status:
  conditions:
  - lastProbeTime: null
    lastTransitionTime: "2025-08-15T13:08:18Z"
    status: "True"
    type: PodReadyToStartContainers
  - lastProbeTime: null
    lastTransitionTime: "2025-08-15T13:08:17Z"
    status: "True"
    type: Initialized
  - lastProbeTime: null
    lastTransitionTime: "2025-08-15T13:08:18Z"
    status: "True"
    type: Ready
  - lastProbeTime: null
    lastTransitionTime: "2025-08-15T13:08:18Z"
    status: "True"
    type: ContainersReady
  - lastProbeTime: null
    lastTransitionTime: "2025-08-15T13:08:17Z"
    status: "True"
    type: PodScheduled
  containerStatuses:
  - allocatedResources:
      cpu: 100m
      memory: 128Mi
    containerID: containerd://45cb22988a025a67da753f4aa62e69493e35a0bd2710c70a15a752ecb5b325e4
    image: docker.io/ikulyk404/busyboxplus:curl
    imageID: docker.io/ikulyk404/busyboxplus@sha256:1b6d0ed7d7b591da2782b7f2c4d9afae1552ecc522ec07e2d74c5054b8be4b5e
    lastState: {}
    name: busybox
    ready: true
    resources:
      limits:
        cpu: 200m
        memory: 256Mi
      requests:
        cpu: 100m
        memory: 128Mi
    restartCount: 0
    started: true
    state:
      running:
        startedAt: "2025-08-15T13:08:18Z"
    user:
      linux:
        gid: 0
        supplementalGroups:
        - 0
        - 1
        - 2
        - 3
        - 4
        - 6
        - 10
        - 11
        - 20
        - 26
        - 27
        uid: 0
    volumeMounts:
    - mountPath: /var/run/secrets/kubernetes.io/serviceaccount
      name: kube-api-access-sjrvk
      readOnly: true
      recursiveReadOnly: Disabled
  hostIP: 172.18.0.3
  hostIPs:
  - ip: 172.18.0.3
  phase: Running
  podIP: 10.244.2.16
  podIPs:
  - ip: 10.244.2.16
  qosClass: Burstable
  startTime: "2025-08-15T13:08:17Z"

  todoapp-daemonset-ktd8k 
  apiVersion: v1
kind: Pod
metadata:
  creationTimestamp: "2025-08-15T13:08:17Z"
  generateName: todoapp-daemonset-
  generation: 1
  labels:
    app: todoapp-daemonset
    controller-revision-hash: 8644898c47
    pod-template-generation: "2"
  name: todoapp-daemonset-ktd8k
  namespace: mateapp
  ownerReferences:
  - apiVersion: apps/v1
    blockOwnerDeletion: true
    controller: true
    kind: DaemonSet
    name: todoapp-daemonset
    uid: 65cf45da-1146-4baf-9473-f2f8f997dc2f
  resourceVersion: "21153"
  uid: e95ccbe3-6899-4176-9935-8f2f2723a2e2
spec:
  affinity:
    nodeAffinity:
      requiredDuringSchedulingIgnoredDuringExecution:
        nodeSelectorTerms:
        - matchFields:
          - key: metadata.name
            operator: In
            values:
            - kind-worker
  containers:
  - args:
    - |
      while true; do
        curl -f http://todoapp-svc-cip.mateapp.svc.cluster.local
        sleep 5
      done
    command:
    - /bin/sh
    - -c
    image: ikulyk404/busyboxplus:curl
    imagePullPolicy: IfNotPresent
    name: busybox
    resources:
      limits:
        cpu: 200m
        memory: 256Mi
      requests:
        cpu: 100m
        memory: 128Mi
    terminationMessagePath: /dev/termination-log
    terminationMessagePolicy: File
    volumeMounts:
    - mountPath: /var/run/secrets/kubernetes.io/serviceaccount
      name: kube-api-access-lhz27
      readOnly: true
  dnsPolicy: ClusterFirst
  enableServiceLinks: true
  nodeName: kind-worker
  preemptionPolicy: PreemptLowerPriority
  priority: 0
  restartPolicy: Always
  schedulerName: default-scheduler
  securityContext: {}
  serviceAccount: default
  serviceAccountName: default
  terminationGracePeriodSeconds: 30
  tolerations:
  - effect: NoExecute
    key: node.kubernetes.io/not-ready
    operator: Exists
  - effect: NoExecute
    key: node.kubernetes.io/unreachable
    operator: Exists
  - effect: NoSchedule
    key: node.kubernetes.io/disk-pressure
    operator: Exists
  - effect: NoSchedule
    key: node.kubernetes.io/memory-pressure
    operator: Exists
  - effect: NoSchedule
    key: node.kubernetes.io/pid-pressure
    operator: Exists
  - effect: NoSchedule
    key: node.kubernetes.io/unschedulable
    operator: Exists
  volumes:
  - name: kube-api-access-lhz27
    projected:
      defaultMode: 420
      sources:
      - serviceAccountToken:
          expirationSeconds: 3607
          path: token
      - configMap:
          items:
          - key: ca.crt
            path: ca.crt
          name: kube-root-ca.crt
      - downwardAPI:
          items:
          - fieldRef:
              apiVersion: v1
              fieldPath: metadata.namespace
            path: namespace
status:
  conditions:
  - lastProbeTime: null
    lastTransitionTime: "2025-08-15T13:08:19Z"
    status: "True"
    type: PodReadyToStartContainers
  - lastProbeTime: null
    lastTransitionTime: "2025-08-15T13:08:17Z"
    status: "True"
    type: Initialized
  - lastProbeTime: null
    lastTransitionTime: "2025-08-15T13:08:19Z"
    status: "True"
    type: Ready
  - lastProbeTime: null
    lastTransitionTime: "2025-08-15T13:08:19Z"
    status: "True"
    type: ContainersReady
  - lastProbeTime: null
    lastTransitionTime: "2025-08-15T13:08:17Z"
    status: "True"
    type: PodScheduled
  containerStatuses:
  - allocatedResources:
      cpu: 100m
      memory: 128Mi
    containerID: containerd://74e356aa178737461a5a346bcbf97c7593037eb2213b33b793155d4ef01e2ed0
    image: docker.io/ikulyk404/busyboxplus:curl
    imageID: docker.io/ikulyk404/busyboxplus@sha256:1b6d0ed7d7b591da2782b7f2c4d9afae1552ecc522ec07e2d74c5054b8be4b5e
    lastState: {}
    name: busybox
    ready: true
    resources:
      limits:
        cpu: 200m
        memory: 256Mi
      requests:
        cpu: 100m
        memory: 128Mi
    restartCount: 0
    started: true
    state:
      running:
        startedAt: "2025-08-15T13:08:18Z"
    user:
      linux:
        gid: 0
        supplementalGroups:
        - 0
        - 1
        - 2
        - 3
        - 4
        - 6
        - 10
        - 11
        - 20
        - 26
        - 27
        uid: 0
    volumeMounts:
    - mountPath: /var/run/secrets/kubernetes.io/serviceaccount
      name: kube-api-access-lhz27
      readOnly: true
      recursiveReadOnly: Disabled
  hostIP: 172.18.0.2
  hostIPs:
  - ip: 172.18.0.2
  phase: Running
  podIP: 10.244.1.13
  podIPs:
  - ip: 10.244.1.13
  qosClass: Burstable
  startTime: "2025-08-15T13:08:17Z"

  todoapp-cronjob-29254396-qx42r
  apiVersion: v1
kind: Pod
metadata:
  creationTimestamp: "2025-08-15T13:16:00Z"
  generateName: todoapp-cronjob-29254396-
  generation: 1
  labels:
    batch.kubernetes.io/controller-uid: ea804196-31ec-4bd6-a0d1-202e258cc363
    batch.kubernetes.io/job-name: todoapp-cronjob-29254396
    controller-uid: ea804196-31ec-4bd6-a0d1-202e258cc363
    job-name: todoapp-cronjob-29254396
  name: todoapp-cronjob-29254396-qx42r
  namespace: mateapp
  ownerReferences:
  - apiVersion: batch/v1
    blockOwnerDeletion: true
    controller: true
    kind: Job
    name: todoapp-cronjob-29254396
    uid: ea804196-31ec-4bd6-a0d1-202e258cc363
  resourceVersion: "21918"
  uid: 5f995a32-8bd8-4014-8ee4-c5990c9f8601
spec:
  containers:
  - command:
    - /bin/sh
    - -c
    - date; curl http://todoapp-svc-cip.mateapp.svc.cluster.local/api/health
    image: ikulyk404/busyboxplus:curl
    imagePullPolicy: IfNotPresent
    name: busybox
    resources: {}
    terminationMessagePath: /dev/termination-log
    terminationMessagePolicy: File
    volumeMounts:
    - mountPath: /var/run/secrets/kubernetes.io/serviceaccount
      name: kube-api-access-rhlc6
      readOnly: true
  dnsPolicy: ClusterFirst
  enableServiceLinks: true
  nodeName: kind-worker2
  preemptionPolicy: PreemptLowerPriority
  priority: 0
  restartPolicy: OnFailure
  schedulerName: default-scheduler
  securityContext: {}
  serviceAccount: default
  serviceAccountName: default
  terminationGracePeriodSeconds: 30
  tolerations:
  - effect: NoExecute
    key: node.kubernetes.io/not-ready
    operator: Exists
    tolerationSeconds: 300
  - effect: NoExecute
    key: node.kubernetes.io/unreachable
    operator: Exists
    tolerationSeconds: 300
  volumes:
  - name: kube-api-access-rhlc6
    projected:
      defaultMode: 420
      sources:
      - serviceAccountToken:
          expirationSeconds: 3607
          path: token
      - configMap:
          items:
          - key: ca.crt
            path: ca.crt
          name: kube-root-ca.crt
      - downwardAPI:
          items:
          - fieldRef:
              apiVersion: v1
              fieldPath: metadata.namespace
            path: namespace
status:
  conditions:
  - lastProbeTime: null
    lastTransitionTime: "2025-08-15T13:16:02Z"
    status: "False"
    type: PodReadyToStartContainers
  - lastProbeTime: null
    lastTransitionTime: "2025-08-15T13:16:00Z"
    reason: PodCompleted
    status: "True"
    type: Initialized
  - lastProbeTime: null
    lastTransitionTime: "2025-08-15T13:16:00Z"
    reason: PodCompleted
    status: "False"
    type: Ready
  - lastProbeTime: null
    lastTransitionTime: "2025-08-15T13:16:00Z"
    reason: PodCompleted
    status: "False"
    type: ContainersReady
  - lastProbeTime: null
    lastTransitionTime: "2025-08-15T13:16:00Z"
    status: "True"
    type: PodScheduled
  containerStatuses:
  - containerID: containerd://3bdbff89d2be7376d8d606ac8784f608d47c3bc9125bcf52f8eee4a31563f157
    image: docker.io/ikulyk404/busyboxplus:curl
    imageID: docker.io/ikulyk404/busyboxplus@sha256:1b6d0ed7d7b591da2782b7f2c4d9afae1552ecc522ec07e2d74c5054b8be4b5e
    lastState: {}
    name: busybox
    ready: false
    resources: {}
    restartCount: 0
    started: false
    state:
      terminated:
        containerID: containerd://3bdbff89d2be7376d8d606ac8784f608d47c3bc9125bcf52f8eee4a31563f157
        exitCode: 0
        finishedAt: "2025-08-15T13:16:00Z"
        reason: Completed
        startedAt: "2025-08-15T13:16:00Z"
    user:
      linux:
        gid: 0
        supplementalGroups:
        - 0
        - 1
        - 2
        - 3
        - 4
        - 6
        - 10
        - 11
        - 20
        - 26
        - 27
        uid: 0
    volumeMounts:
    - mountPath: /var/run/secrets/kubernetes.io/serviceaccount
      name: kube-api-access-rhlc6
      readOnly: true
      recursiveReadOnly: Disabled
  hostIP: 172.18.0.3
  hostIPs:
  - ip: 172.18.0.3
  phase: Succeeded
  podIP: 10.244.2.17
  podIPs:
  - ip: 10.244.2.17
  qosClass: BestEffort
  startTime: "2025-08-15T13:16:00Z"