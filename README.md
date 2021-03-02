# infra-ci-cdn-refresh

A cdn refresh ci of summer-ospp for github action.

## USE

```
- name: Refresh
  uses: summer-ospp/infra-ci-cdn-refresh@main
  env:
    CDN_AK: ${{ secrets.HOMEPAGE_CDN_AK }}
    CDN_SK: ${{ secrets.HOMEPAGE_CDN_SK }}
    CDN_REFRESH_URLS: ${{ secrets.HOMEPAGE_CDN_REFRESH_URLS }}
    CDN_REFRESH_TYPE: ${{ secrets.HOMEPAGE_CDN_REFRESH_TYPE }}
```

## Configuration

| Key | Value | Suggested Type | Required | Default |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| CDN_PROJECTID | Project ID | env | No | '' |
| CDN_CLOUD | CLoud | env | No | myhuaweicloud.com |
| CDN_REGION | Region | env| No | cn-north-1 |
| CDN_AK | Access key id | secret env | Yes | N/A |
| CDN_SK | Secret access key | secret env | Yes | N/A |
| CDN_REFRESH_URLS | Refresh URL | env | Yes | N/A |
| CDN_REFRESH_TYPE | directory or file | env | Yes | N/A |

