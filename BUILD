python_requirement_library(
  name='pants-req',
  requirements=[
    python_requirement('pantsbuild.pants==0.0.24'),

    # This is a hack to work around the fact we have no 4.x platform specific eggs uploaded
    # to the cheeseshop.
    python_requirement('coverage==3.7.1'),
  ]
)

python_binary(
  name='pants',
  entry_point='pants.bin.pants_exe:main',
  platforms=[
    'current',
    'linux-x86_64',
    'macosx-10.4-x86_64',
  ],
  dependencies=[
    ':pants-req',
  ]
)
