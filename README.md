### Example Usage:
```
module "vmimport" {
  source = "StratusGrid/terraform-aws-iam-role-vmimport"
  version = "1.0.0"
  # source = "github.com/StratusGrid/terraform-aws-vmimport"
  image_bucket_name = "my-bucket-of-images"
  input_tags  = "${merge(local.common_tags,
    map(
    )
  )}"
}
```