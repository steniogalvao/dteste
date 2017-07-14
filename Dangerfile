# boolean para verificar se ocorreram mudanças na aplicação
#has_app_changes = !(git.modified_files.grep(/src/main/java/).empty?)
has_app_changes = !(git.modified_files.grep("/src/main/java/br/com/vsgdev/dtest").empty?)
# boolean para verificar se ocorreram mudanças nos testes
#has_test_changes = !git.modified_files.grep(/src/test/java/).empty?


# Alertando sobre a importancia dos testes
if has_app_changes
    warn ("Talvez você deva alterar/implementar testes para as suas alterções.")    
end

# Warn when there is a big PR
warn("Big PR") if git.lines_of_code > 1

warn("Just testing a damn warning")

