# frozen_string_literal: true

# -*- mode: ruby -*-
# vi: set ft=ruby :

# This file is to hook the drupal-vm Vagrantfile, and init some variables.
# If you know how to use drupal-vm, you can directly load drupal-vm Vagrantfile.

# The absolute path to the root directory of the project. Both Drupal VM and
# the config file need to be contained within this path.
ENV['DRUPALVM_PROJECT_ROOT'] = ENV['YIIPALVM_PROJECT_ROOT'] || "#{__dir__}";

# The relative path from the project root to the config directory where you
# placed your config.yml file.
ENV['DRUPALVM_CONFIG_DIR'] = ENV['YIIPALVM_CONFIG_DIR'] || "box"

# The relative path from the project root to the directory where Drupal VM is located.
ENV['DRUPALVM_DIR'] = ENV['VENDOR_DIR'] ? "#{ENV['VENDOR_DIR']}/geerlingguy/drupal-vm" : "vendor/geerlingguy/drupal-vm"

# The vm environment.
if ENV['YIIPALVM_ENV']
  ENV['DRUPALVM_ENV'] = ENV['YIIPALVM_ENV']
end

# Load the real Vagrantfile
load "#{ENV['DRUPALVM_PROJECT_ROOT']}/#{ENV['DRUPALVM_DIR']}/Vagrantfile"
