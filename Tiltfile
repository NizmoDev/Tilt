docker_build(
    'my-app-image',
    '.'
)

k8s_yaml(['deployment.yaml', 'service.yaml'])

k8s_resource(
    'my-app',
    port_forwards=8085
)