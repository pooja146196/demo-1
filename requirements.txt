import pkg_resources

for dist in pkg_resources.working_set:
    if '.egg' in dist.location:
        print(f"{dist.project_name}=={dist.version} from {dist.location}")
