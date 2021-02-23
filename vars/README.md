# Ansible S3

### Steps to use

1. In order to run the playbook, ensure you have AWS Credentials setup in your machine.

2. Follow the following steps to run the playbook.

```

To Create a bucket:

$ ansible-playbook playbook.yml -e "state=present, bucket_name=test-bucket-s3-krupa"

To Delete a bucket:

$ ansible-playbook playbook.yml -e "state=absent, bucket_name=test-bucket-s3-krupa"


```

3. You can skip the `-e` and run it simply by `ansible-playbook playbook.yml`. Doing so will require changes in the `main.yml` file present in vars folder.


### Folder Structure

```

.
├── playbook.yml
└── vars
    ├── README.md
    └── main.yml

1 directory, 3 files


```
